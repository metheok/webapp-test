<template>
  <div class="container">
    <div class="details">
      <div class="card">
        <div class="card-left">
          <div class="icon-wrapper" style="background-color: #fee7cc;">
            <span class="material-icons" style="font-size: 24px;">
              article
            </span>
          </div>
          <div class="content-wrapper">
            <div class="title">Articles Posted</div>
            <div class="subtitle">80</div>
          </div>
        </div>
        <div class="card-right">
          <span class="material-icons">
            keyboard_arrow_right
          </span>
        </div>
      </div>
      <div class="card">
        <div class="card-left">
          <div class="icon-wrapper" style="background-color: #d8ddfa;">
            <span class="material-icons" style="font-size: 24px;">
              thumb_up_alt
            </span>
          </div>
          <div class="content-wrapper">
            <div class="title">Claps This Week</div>
            <div class="subtitle">1.5K</div>
          </div>
        </div>
        <div class="card-right">
          <span class="material-icons">
            keyboard_arrow_right
          </span>
        </div>
      </div>
      <div class="card">
        <div class="card-left">
          <div class="icon-wrapper" style="background-color: #e5e5e5;">
            <span class="material-icons" style="font-size: 24px;">
              group
            </span>
          </div>
          <div class="content-wrapper">
            <div class="title">New Followers This Week</div>
            <div class="subtitle">972</div>
          </div>
        </div>
        <div class="card-right">
          <span class="material-icons">
            keyboard_arrow_right
          </span>
        </div>
      </div>

      <div class="followers">
        <div class="follow-heading">
          <h4 class="follow-head">Followers</h4>
          <p class="view-all">View All</p>
        </div>

        <div class="followers-wrapper">
          <a class="followers" href="#">
            <img
              class="follower-img"
              src="https://i.pinimg.com/236x/2d/0a/c5/2d0ac5f5a8380ba790cb88845ea4484c.jpg"
            />
            <p>James May</p>
          </a>
          <a class="followers" href="#">
            <img
              class="follower-img"
              src="https://i.pinimg.com/236x/d6/f8/14/d6f814dfb3a5d372fa8eab3558f35047.jpg"
            />
            <p>Paul Mcartney</p>
          </a>
          <a class="followers" href="#">
            <img
              class="follower-img"
              src="https://i.pinimg.com/236x/74/f5/a0/74f5a0511beb735dae7350f1526ff215.jpg"
            />
            <p>Jhonny cash</p>
          </a>
        </div>
      </div>
      <div class="banner">
        <span class="description"
          >Buy <span class="emphasis">Pro Account</span> to Explore Premium
          Features</span
        >
        <button class="button">
          Purchase Now
        </button>
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style scoped>
@import url("https://fonts.googleapis.com/icon?family=Material+Icons");

.container {
  display: flex;
  flex-direction: column;
  margin: 25px 20px;
  flex: 1;
}

.details {
  background-color: #f7f7f7;
  padding: 30px;
  border-radius: 25px;
  margin-top: 50px;
}

.card {
  width: 100%;
  height: 70px;
  background-color: white;
  border-radius: 15px;
  display: flex;
  flex-direction: row;
  justify-content: space-between;
  padding: 15px;
  box-sizing: border-box;
  margin-bottom: 30px;
  -webkit-box-shadow: 0px 1px 1px 1.5px rgba(0, 0, 0, 0.12);
  -moz-box-shadow: 0px 1px 1px 1.5px rgba(0, 0, 0, 0.12);
  box-shadow: 0px 1px 1px 1.5px rgba(0, 0, 0, 0.12);
}

.card > .card-left {
  width: auto;
  height: auto;
  display: flex;
  flex-direction: row;
}

.card > .card-left > .icon-wrapper {
  width: 40px;
  height: 40px;
  border-radius: 10px;
  margin-right: 10px;
  display: flex;
  justify-content: center;
  align-items: center;
}

.card > .card-left > .content-wrapper {
  display: flex;
  flex-direction: column;
}

.title {
  font-size: 14px;
  font-family: "Lato", sans-serif;
}

.subtitle {
  font-size: 20px;
  font-family: "Lato", sans-serif;
  font-weight: 700;
}

.card > .card-right {
  background-color: #efefef;
  align-self: center;
  border-radius: 10px;
  display: flex;
  justify-content: center;
}

.banner {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  background-color: white;
  background-size: 100%;
  background-position: center;
  background-image: url(https://upload.wikimedia.org/wikipedia/commons/thumb/0/0e/Globe_centered_in_the_Atlantic_Ocean_%28green_and_grey_globe_scheme%29.svg/1200px-Globe_centered_in_the_Atlantic_Ocean_%28green_and_grey_globe_scheme%29.svg.png);
  padding: 60px 0;
  margin-top: 30px;
  border-radius: 20px;
}

.banner > .description {
  font-family: "Lato", sans-serif;
  color: #383135;
  margin: 0px 20% 0px;
  text-align: center;
  overflow: hidden;
}

.emphasis {
  color: #383135;
  font-weight: 700;
}

.button {
  margin-top: 20px;
  border-width: 0px;
  background-color: #383135;
  color: white;
  font-family: "Lato", sans-serif;
  padding: 10px 15px;
  border-radius: 8px;
}
button {
  all: unset;
}

button:hover,
button:focus {
  background: #000;
}

button:active {
  transform: scale(0.99);
}

/*followers cards*/

.follow-heading {
  display: flex;
  justify-content: space-between;
  align-items: center;
}

.followers-wrapper {
  display: flex;
}
.followers {
  margin: 4px 8px;
}
.followers img {
  height: 90px;
  width: 90px;
  border-radius: 15px;
}
.followers a {
  text-decoration: none;
}
a > p {
  position: relative;
  text-align: center;
  background-color: rgba(0, 0, 0, 0.22);

  font-size: 10px;
  color: whitesmoke;
  bottom: 35px;
}
@media (max-width: 768px) {
  .container {
    width: 790px;
    margin: 25px 15px;
  }
}
</style>
