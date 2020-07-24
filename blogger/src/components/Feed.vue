<template>
  <div class="intro">
    <div class="left-side"></div>
    <div class="main">
      <div class="top2">
        <input class="search" type="text" placeholder="Search..." />
      </div>
      <div class="top1">
        <h2>Hi John Doe.</h2>
        <p>
          Welcome back John Doe. We are glad you are here. Inspire the best work
          in people, enabling them to achieve their goals.
        </p>
        <div class="img">
          <img src="https://picsum.photos/200" alt="img" />
        </div>

        <button class="button">View Details</button>
      </div>

      <div class="mid">
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
                In essence, typography is the art of arranging letters and text
                in a way that _
              </p>
            </div>
          </div>
          <div class="column">
            <div class="card">
              <h4>Color Palatte</h4>
              <p>
                The best way to use a scheme like this is to use one color as
                the primary _
              </p>
            </div>
          </div>
        </div>
      </div>
    </div>
    <div class="right-side"></div>
    <List></List>
  </div>
</template>

<script>
import List from "@/components/List.vue";
export default {
  components: {
    List,
  },
};
</script>

<style scoped></style>
