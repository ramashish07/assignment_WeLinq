<template>
  <div class="sidebarSec">
    <div class="logo">
      <img src="../assets/welinq.png" style="height: 80px; width: 80px" />
    </div>
    <div class="ss2">
      <div class="box">
        <img
          src="../assets/home.png"
          style="
            height: 17px;
            width: 17px;
            vertical-align: middle;
            margin-right: 5px;
          "
        />
        Home
      </div>
      <div class="box">
        <img
          src="../assets/Variant3.png"
          style="
            height: 17px;
            width: 17px;
            vertical-align: middle;
            margin-right: 5px;
          "
        />
        My Sessions
      </div>
      <div class="box">
        <img
          src="../assets/therapist.png"
          style="
            height: 17px;
            width: 17px;
            vertical-align: middle;
            margin-right: 5px;
            border: 1px solid #fff; /* Add a border to the image */
          "
        />
        Therapist
      </div>

      <div class="box">
        <img
          src="../assets/quiz.png"
          style="
            height: 17px;
            width: 17px;
            vertical-align: middle;
            margin-right: 5px;
          "
        />
        Quizzes
      </div>
      <div class="box">
        <img
          src="../assets/web.png"
          style="
            height: 17px;
            width: 17px;
            vertical-align: middle;
            margin-right: 5px;
          "
        />
        Webinars
      </div>
      <div class="box">
        <img
          src="../assets/profile.png"
          style="
            height: 17px;
            width: 17px;
            vertical-align: middle;
            margin-right: 5px;
          "
        />
        Profile
      </div>
    </div>
    <div class="cal">
      <img src="../assets/cal.png" height="150px" width="150px" />
    </div>
  </div>
</template>

<script>
export default {
  // You can add component-specific logic here if needed
};
</script>

<style scoped>
/* Add styling for the sidebar here */
.sidebarSec {
  width: 15vw;
  height: 100%;
  flex-shrink: 0;
  display: flex;
  gap: 35px;
  align-items: center;
  flex-direction: column;
  background: #fff;
  padding: 16px;
}
.logo {
  display: flex;
  /* padding: 20px 40px; Adjust padding as needed */
  align-items: center;
  justify-content: center;
  border-radius: 20px;
  background: #f4f5ff;
  width: 100%;
  height: 200px; /* Adjust the height value as needed */
  gap: 10px;
}
.ss2 {
  display: flex;
  padding: 5px 30px;
  align-items: center;
  gap: 10px;
  border-radius: 10px;
  background: #fff;
}
.cal {
  height: 200px;
  width: 1;
  justify-items: center;
  align-items: center;
}
.box {
  color: #848484;
  font-family: Poppins;
  font-size: 14px;
  font-style: normal;
  font-weight: 400;
  line-height: 131%; /* 23.58px */
  margin-top: 5px;
}
.ss1 {
  width: vw;
  padding: 30px;
  /* padding-left: 0;
  padding-right: 0; */
  margin-top: 25px;
  margin-right: 25px;
  margin-left: 25px;

  display: flex;
  align-items: center;
  justify-content: center;
  border-radius: 8px;
  background: #f4f5ff;
  display: inline-flex;
  padding: 40px 80px;
  align-items: flex-start;
  gap: 10px;
}
.ss1 > img {
  height: 60px;
  width: 60px;
}
.ss2 {
  display: flex;
  flex-direction: column;
  align-items: flex-start;
  justify-content: center;
  gap: 8px;
  width: 16vw;
}
.ss2 > a {
  width: 100%;
  font-size: 14px;
  display: flex;
  flex: none;
  align-items: center;
  justify-content: start;
  outline: none;
  border: none;
  border-radius: 4px;
  cursor: pointer;
  font-weight: 600;
}
.ss2 > a > * {
  margin-left: 24px;
}
.ss2 > a:hover {
  background: purple;
  color: white;
}
.ss3 {
  width: 16vw;
  padding: 0;
  margin: 0;
  display: flex;
  align-items: center;
  justify-content: center;
  overflow: hidden;
  border-radius: 8px;
  background: #e5e7ff;
}
</style>
