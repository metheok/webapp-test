<template>
  <div class="main">
    <div class="top">
      <h4>List of Blogs</h4>
      <p>Filter By:</p>
      <div class="sta-class">
        <select id="status" v-model="filterStatus" name="Status">
          <option value="" disabled selected>Status</option>
          <option value="">All </option>
          <option value="published">Published</option>
          <option value="draft">Draft</option>
          <option value="deactivated">Deactivated</option>
        </select>
      </div>
      <div class="date-class">
        <select id="date" v-model="filterYear" name="Date">
          <option value="" disabled selected>Date</option>
          <option value="">All</option>
          <option value="2015">2015</option>
          <option value="2016">2016</option>
          <option value="2017">2017</option>
          <option value="2018">2018</option>
          <option value="2019">2019</option>
          <option value="2020">2020</option>
        </select>
      </div>
    </div>
    <table>
      <colgroup>
        <col width="10%" />
      </colgroup>

      <thead>
        <tr>
          <th>Date</th>
          <th>Title</th>
          <th>Status</th>
        </tr>
      </thead>
      <tbody>
        <tr v-for="post in filteredPosts" :key="post.id">
          <td>{{ post.date }}</td>
          <td>{{ post.title }}</td>
          <td>{{ post.status }}</td>
        </tr>
        <tr></tr>
      </tbody>
    </table>
  </div>
</template>

<script>
import axios from "axios";
export default {
  data: function() {
    return {
      posts: [],
      filterStatus: "",
      filterYear: ""
    };
  },
  mounted() {
    axios
      .get("https://my-json-server.typicode.com/orzel-bielik/test/posts")
      .then(res => {
        this.posts = res.data;
        this.posts.forEach((element, index) => {
          this.posts[index].date = element.date.split("-", 1)[0];
        });
      })
      .catch(err => {
        console.log(err);
      });
  },

  computed: {
    filteredPosts: function() {
      return this.posts.filter(post => {
        return (
          post.status.match(this.filterStatus) &&
          post.date.match(this.filterYear)
        );
      });
    }
  }
};
</script>

<style scoped>
body {
  color: #444;
}

.main {
  margin: 30px auto;
  text-align: left;
}

table {
  background: #f5f5f5;
  border-collapse: separate;
  box-shadow: inset 0 1px 0 #fff;
  font-size: 12px;
  line-height: 22px;
  width: 95%;
  table-layout: auto;
}

.top {
  display: flex;
}

th {
  background: rgb(219, 219, 219);
  border: none;
  border-radius: 2px;
  color: #000;
  font-weight: bold;
  padding: 10px 15px;
  position: relative;
}

td {
  padding: 10px 15px;
  position: relative;
  transition: all 300ms;
}

select {
  padding: 10px 15px;
  margin: 0 5px;
  border: none;
  outline: none;
  border-radius: 6px;
  background: rgb(230, 229, 229);
}

.sta-class,
.date-class {
  align-self: center;
}
.top h4 {
  margin-left: 20px;
  margin-right: 52%;
  align-self: flex-start;
}
.top p {
  align-self: center;
  font-style: italic;
  font-size: 0.8rem;
}
</style>
