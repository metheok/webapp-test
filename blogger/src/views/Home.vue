<template>
  <div class="home">
    <Nav-Bar />
    <Feed />
    <Details />
  </div>
</template>

<script>
// @ is an alias to /src

import Feed from "@/components/Feed.vue";
import Details from "@/components/Details.vue";
import NavBar from "@/components/NavBar.vue";

export default {
  name: "Home",
  components: {
    Details,
    Feed,
    NavBar,
  },
};
</script>
<style scoped>
.home {
  display: flex;
}
</style>
