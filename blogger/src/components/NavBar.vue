<template>
  <div id="nav">
    <router-link to="/">
      <img class="icon-img" src="../assets/icons/svg/001-home.svg" alt="" />
    </router-link>
    <router-link to="/"
      ><img class="icon-img" src="../assets/icons/svg/002-app.svg" alt=""
    /></router-link>
    <router-link to="/"
      ><img class="icon-img" src="../assets/icons/svg/003-calendar.svg" alt=""
    /></router-link>
    <router-link to=""
      ><img class="icon-img" src="../assets/icons/svg/004-shop.svg" alt=""
    /></router-link>
    <router-link to=""
      ><img class="icon-img" src="../assets/icons/svg/005-settings.svg" alt=""
    /></router-link>
    <router-link to=""
      ><img
        class="icon-img set"
        src="../assets/icons/svg/006-back-arrow.svg"
        alt=""
    /></router-link>
  </div>
</template>

<script>
export default {};
</script>

<style scoped>
#nav {
  display: flex;
  flex-direction: column;
  position: sticky;
  background-color: #383135;
  width: 75px;
  margin: 20px 20px;
  border-radius: 23px;
}
.icon-img {
  width: 18px;
  height: 18px;
  margin: 20px 28px;
}
.icon-img.set {
  margin-top: 150px;
}
</style>
