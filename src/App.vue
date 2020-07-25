<template>
  <div id="app">
    <div id="appli">
      <NavBar />
      <router-view class="feed"></router-view>
      <Details />
    </div>
    <div class="top-section-container">
      <div class="notity-container">
        <a href="#"
          ><img
            class="notify"
            src="https://www.flaticon.com/premium-icon/icons/svg/3106/3106685.svg"
        /></a>
      </div>
      <div class="language-sel-container">
        <select name="" id="dropdown">
          <option value="EN">EN</option>
          <option value="ESP">ESP</option>
          <option value="POR">POR</option>
        </select>
      </div>
      <div class="user-name-container">
        <h4>John Doe</h4>
        <p>John Doe</p>
      </div>
      <div class="profile-pic-container">
        <img
          src="https://upload.wikimedia.org/wikipedia/commons/thumb/9/9c/Jay-Z_%40_Shawn_%27Jay-Z%27_Carter_Foundation_Carnival_%28crop_2%29.jpg/220px-Jay-Z_%40_Shawn_%27Jay-Z%27_Carter_Foundation_Carnival_%28crop_2%29.jpg"
          alt="John Doe"
        />
      </div>
    </div>
  </div>
</template>
<script>
// @ is an alias to /src
import NavBar from "@/components/NavBar.vue";
import Details from "@/components/Details.vue";

export default {
  components: {
    NavBar,
    Details
  }
};
</script>
<style>
@import url("https://fonts.googleapis.com/css2?family=Lato:wght@400;700;900&display=swap");

body {
  width: 100%;
  padding: 0;
  margin: 0;
  background-color: white;
  color: #383135;
  font-family: "Lato", sans-serif;
}
h1,
h2,
h3,
h4 {
  margin: 0;
}

.feed {
  margin-left: 100px;
}

/*top section container */
#appli {
  display: flex;
  flex-direction: row;
}

.top-section-container {
  height: 40px;
  width: 300px;
  position: absolute;
  display: flex;
  flex-direction: row;
  justify-content: flex-end;
  top: 10px;
  right: 1px;
  margin: 5px 0;
}
.notify-container {
  width: 20%;
  float: left;
  height: inherit;
  margin: 0 8px;
}
.notify {
  float: left;
  width: 30px;
  height: inherit;
  margin-top: 16px;
}
.notify:hover {
  background-color: #e0e2e4;
  transform: scale(1.2);
  border-radius: 50%;
}
.language-sel-container {
  height: inherit;
  margin: 0 8px;
  width: 30px;
  margin-top: 20px;
}
.dropdown {
  outline: none;
  border-color: none;
}

.user-name-container {
  margin: 15px 4px 0px 45px;
  color: gray;
}
.user-name-container h4,
.user-name-container p {
  padding: 0;
  margin: 0;
  font-size: 0.8rem;
}

.profile-pic-container {
  height: inherit;
  margin: 0 0;
  padding: 0;
}
.profile-pic-container img {
  height: 50px;
  width: 50px;
  border-radius: 50%;
  border-color: black;
}
@media (max-width: 868px) {
  .feed {
    margin-left: 0px;
  }
  #appli {
    display: block;
    margin-top: 100px;
  }
  .top-section-container {
    top: 110px;
  }
}
</style>
