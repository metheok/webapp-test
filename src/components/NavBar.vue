<template>
  <div id="nav">
    <router-link to="/">
      <img class="icon-img" src="../assets/icons/svg/001-home.svg" alt="" />
    </router-link>
    <router-link to="more"
      ><img class="icon-img" src="../assets/icons/svg/002-app.svg" alt=""
    /></router-link>
    <router-link to="calendar"
      ><img class="icon-img" src="../assets/icons/svg/003-calendar.svg" alt=""
    /></router-link>
    <router-link to="shop"
      ><img class="icon-img" src="../assets/icons/svg/004-shop.svg" alt=""
    /></router-link>
    <router-link to="settings"
      ><img class="icon-img" src="../assets/icons/svg/005-settings.svg" alt=""
    /></router-link>
    
      <img
        class="icon-img set"
        src="../assets/icons/svg/006-back-arrow.svg"
        alt=""
    />
  </div>
</template>

<script>
export default {};
</script>

<style scoped>
#nav {
  display: flex;
  flex-direction: column;
  position: fixed;
  background-color: #383135;
  width: 75px;
  height: 570px;
  margin: 20px 20px;
  border-radius: 23px;
  padding: 8px 0;
}
.router-link-active {
  background-color: grey;
  border: none;

  border-radius: 100%;
}
.icon-img {
  width: 18px;
  height: 18px;
  margin: 20px 28px;
  padding: 12px 0;
}
.icon-img.set {
  margin-top: 100%;
}
@media (max-width: 868px) {
  #nav {
    flex-direction: row;
    height: 75px;
    width: 95%;
    top: 0px;
    justify-content: space-around;
    align-items: center;
    padding: 0px 0;
  }
  .icon-img.set {
    margin-top: 18px;
    padding: 8px 0;
  }
}
</style>
