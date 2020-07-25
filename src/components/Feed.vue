<template>
  <div class="main">


    <div class="top">
      <img
          class="searchicon"
        src="https://image.flaticon.com/icons/svg/1086/1086933.svg"
        />
 
      <input class="search" type="text" placeholder="Search" />
    </div>


    <div class="intro">
       <div class="text">
               <h2>Hi John Doe.</h2>
      <p>
        Welcome back John Doe. We are glad you are here. Inspire the best work
        in people, enabling them to achieve their goals.
      </p>

      <button class="button">View Details</button>
       </div>
       <div class="image"> 
         <img class ="material-pic" src="https://propeller.in/website/wp-content/themes/propeller/assets/landing-page/images/developer.svg"/>
       </div>

       
      

      
    </div>


    <div class="trending">
      <h3>Trending Blogs</h3>
      <div class="row">
        <div class="column">
          <div class="card">
            <h4>Prototyping</h4>
            <p>
              A prototype is an early sample, model or release of a product
              built to test a _
            </p>
          </div>
        </div>
        <div class="column" style=" color:white">
          <div class="card" style=" background-color: #383135">
            <h4>Typography</h4>
            <p>
              In essence, typography is the art of arranging letters and text in
              a way that _
            </p>
          </div>
        </div>
        <div class="column">
          <div class="card">
            <h4>Color Palatte</h4>
            <p>
              The best way to use a scheme like this is to use one color as the
              primary _
            </p>
          </div>
        </div>
      </div>
    </div>

    <List></List>
  </div>
</template>

<script>
import List from "@/components/List.vue";
export default {
  components: {
    List
  }
};
</script>

<style scoped>
.main {
  width: 55%;
  margin: 20px;
  display: flex;
  flex-direction: column;
}

/*searchbox styling*/

.top {
  width: 60%;
  border: hidden;
  background-color: #f7f7f7;
  height: 40px;
  border-radius: 15px;
  display: flex;
  justify-content: flex-start;
}
.top > .search {
  border: hidden;
  background-color: #f7f7f7;
  margin: 10px;
  font-weight: 550;
}

.top > .searchicon {
  width: 25px;
  margin-left: 20px;
}

/*john doe intro style */

.intro {
  background-color: #f7f7f7;
  border-radius: 15px;
  margin: 30px 0;
  display: flex;
  flex-direction: row;
}
.intro .text {
  display: flex;
  flex-direction: column;
  padding: 20px 30px;
}

.intro img {
  width: 220px;
}

.intro .button {
  width: 150px;
  border-width: 0px;
  background-color: #383135;
  color: white;
  font-family: "Lato", sans-serif;
  padding: 10px 15px;
  border-radius: 8px;
}

/*trending blogs*/
</style>
