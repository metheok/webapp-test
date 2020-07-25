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
        <img
          class="material-pic"
          src="https://propeller.in/website/wp-content/themes/propeller/assets/landing-page/images/developer.svg"
        />
      </div>
    </div>

    <div class="trending">
      <h3>Trending Blogs</h3>
      <p>View all</p>
      <div class="row">
        <div class="column">
          <div class="card">
            <h4>Prototyping</h4>
            <p>
              A prototype is an early sample, model or release of a product
              built to test a _
            </p>
            <div class="blog-claps">
              <img
                class="clapper-img p1"
                src="https://i.pinimg.com/236x/bf/8f/09/bf8f0936f18208ba22c2015f5d5870f5.jpg"
              />
              <img
                class="clapper-img p2"
                src="https://i.pinimg.com/236x/e1/e0/1a/e1e01a5afed2356d202aa9a28cd6b260.jpg"
              />
              <img
                class="clapper-img p3"
                src="https://i.pinimg.com/236x/5e/6c/d4/5e6cd40eae487281b45ea9968130d276.jpg"
              />
              <img
                class="clapper-img p4"
                src="https://i.pinimg.com/236x/3d/05/76/3d0576f36d5c321a47f36d6000351df4.jpg"
              />
            </div>

            <div class="clap">
              <img
                class="clap-icon"
                src="https://image.flaticon.com/icons/svg/2636/2636674.svg"
              />
              <b> <p class="clapper-number">1.2K</p></b>
            </div>
          </div>
        </div>

        <div class="column" style=" color:white">
          <div class="card" style=" background-color: #383135">
            <h4>Typography</h4>
            <p>
              In essence, typography is the art of arranging letters and text in
              a way that _
            </p>
            <div class="blog-claps">
              <img
                class="clapper-img p1"
                src="https://i.pinimg.com/236x/bf/8f/09/bf8f0936f18208ba22c2015f5d5870f5.jpg"
              />
              <img
                class="clapper-img p2"
                src="https://i.pinimg.com/236x/e1/e0/1a/e1e01a5afed2356d202aa9a28cd6b260.jpg"
              />
              <img
                class="clapper-img p3"
                src="https://i.pinimg.com/236x/5e/6c/d4/5e6cd40eae487281b45ea9968130d276.jpg"
              />
              <img
                class="clapper-img p4"
                src="https://i.pinimg.com/236x/3d/05/76/3d0576f36d5c321a47f36d6000351df4.jpg"
              />
            </div>

            <div class="clap">
              <img
                class="clap-icon"
                src="https://image.flaticon.com/icons/svg/2636/2636674.svg"
              />
              <b> <p class="clapper-number">1.5K</p></b>
            </div>
          </div>
        </div>
        <div class="column">
          <div class="card">
            <h4>Color Palatte</h4>
            <p>
              The best way to use a scheme like this is to use one color as the
              primary _
            </p>
            <div class="blog-claps">
              <img
                class="clapper-img p1"
                src="https://i.pinimg.com/236x/bf/8f/09/bf8f0936f18208ba22c2015f5d5870f5.jpg"
              />
              <img
                class="clapper-img p2"
                src="https://i.pinimg.com/236x/e1/e0/1a/e1e01a5afed2356d202aa9a28cd6b260.jpg"
              />
              <img
                class="clapper-img p3"
                src="https://i.pinimg.com/236x/5e/6c/d4/5e6cd40eae487281b45ea9968130d276.jpg"
              />
              <img
                class="clapper-img p4"
                src="https://i.pinimg.com/236x/3d/05/76/3d0576f36d5c321a47f36d6000351df4.jpg"
              />
            </div>

            <div class="clap">
              <img
                class="clap-icon"
                src="https://image.flaticon.com/icons/svg/2636/2636674.svg"
              />
              <b> <p class="clapper-number">1.1K</p></b>
            </div>
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
  width: 800px;
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
  outline: none;
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

.intro .button:hover,
.intro .button:focus {
  background: #000;
}
/*trending blogs*/

.trending > h3,
.trending > p {
  display: inline;
}
.trending > p {
  float: right;
}

.trending .row {
  display: flex;
  flex-direction: row;
  padding: 30px 0;
}

.card p {
  font-size: 0.8rem;
}
.card {
  background-color: #f7f7f7;
  border-radius: 15px;
  padding: 10px;
  margin: 5px;
  height: 140px;
}
.blog-claps {
  float: left;
  width: %;
  height: 50%;
}
.p2 {
  position: relative;
  right: 12px;
}
.p3 {
  position: relative;
  right: 25px;
}
.p4 {
  display: inline;
  position: relative;
  right: 35px;
}
.clapper-img {
  border-radius: 50%;
  border: 3px solid #fff;
  width: 30px;
  height: 30px;
}
.clap {
  float: right;

  height: 50%;
}

.clap-icon {
  display: inline;
  float: left;
  width: 20px;
  height: 20px;
}
.clapper-number {
  display: inline;
  float: right;
}
@media (max-width: 768px) {
  .feed {
    margin-left: 0px;
  }
  #appli {
    display: block;
  }
  .top {
    width: 40%;
  }
}
@media (max-width: 600px) {
  .top {
    position: relative;
    top: 60px;
    width: 60%;
  }
  .intro {
    margin-top: 80px;
  }
}
</style>
