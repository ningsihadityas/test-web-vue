<template>
  <div class="bg-img">
    <div class="b">
      <div class="f">
        <div class="topnav">
          <img justify-center align-center src="@/assets/logo-medco.png" />

          <div>
            <a href="#home">Home</a>
            <a href="#about-us">About Us</a>
            <a href="#business-activity">Business Activity</a>
            <a href="#contact">Contact</a>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: "HomePageHeader",
  components: {},
};
</script>

<style lang="scss" scoped>
/* Position the navbar container inside the image */
/* The navbar */
/* Navbar links */
.bg-img {
  background-image: url("@/assets/medco.png");
  min-height: 380px;
  background-position: center;
  background-repeat: no-repeat;
  background-size: cover;
  position: relative;

  .b {
    background: rgba(0, 0, 0, 0.2);
    color: #fff;
    min-height: 380px;
    .f {
      min-height: 75px;
      padding-right: 0%;
      padding-left: 0%;
      backdrop-filter: blur(2px);
      background: rgba(0, 0, 0, 0.2);
      color: #fff;

      .topnav {
        padding: 15px;
        overflow: hidden;
        //transparant background colour

        width: 100%;
        text-align: right;
        div {
          margin-top: 15px;
          padding-left: 25px;
        }
        img {
          float: left;
          width: 150px; 
          margin-left: 100px;
        }
        a {
          color: #f2f2f2;
          padding: 14px 16px;
          text-decoration: none;
          font-size: 17px;
          &:hover {
            background-color: #ddd;
            color: black;
          }
        }
      }
    }
  }
}

.container-xxl {
  max-width: 100%;
}
.container-xl {
  max-width: 100%;
}
.container-lg {
  max-width: 100%;
}
.container-md {
  max-width: 100%;
}
.container-sm {
  max-width: 100%;
}
.container {
  max-width: 100%;
}
</style>
