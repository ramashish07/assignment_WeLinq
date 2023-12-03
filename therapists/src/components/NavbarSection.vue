<!-- src/components/Navbar.vue -->

<template>
  <nav style="padding: 5px 15px" class="navbar">
    <div class="nb1">Therapists</div>
    <div class="cont_nb">
      <div class="imagecontainer">
        <img
          class="imagecontainer_image"
          src="../assets/Group_icon.svg "
          alt="icon"
        />
      </div>

      <div class="nb4">
        <div class="nb5">
          <img
            src="../assets/search.png"
            style="
              margin-left: 20px;
              margin-right: 10px;
              height: 25px;
              width: 25px;
            "
          />
          Search for session
        </div>
      </div>
      <div class="imagecontainer">
        <img src="../assets/icon3.png " alt="icon" />
      </div>
      <div class="imagecontainer">
        <img src="../assets/icon4.png " alt="icon" />
      </div>
    </div>
  </nav>
</template>
<!-- <template>
  <div style="display: flex; justify-content: space-between">
    <div>sdvhfjb</div>
    <div>sdvhfjb</div>
  </div>
</template> -->

<script>
export default {};
</script>

<style scoped>
/* Add styling for the navbar here */
.navbar {
  display: flex;
  justify-content: space-between;
  align-items: center;
  width: 85vw;
}
.nb1 {
  display: flex;
  flex-shrink: 0;
  color: #292c30;
  font-family: Poppins;
  font-size: 24px;
  /* width: 40vw; */
  align-items: flex-start;
  font-style: normal;
  font-weight: 600;
  line-height: normal;
  gap: 200px;
}
.cont_nb {
  display: flex;
  align-items: center;
  justify-content: center;
  gap: 20px;
}
.imagecontainer {
  width: 50px;
  height: 50px;
  border-radius: 50%;
  flex-shrink: 0;
  background: #fff;
  display: flex;
  justify-content: center;
  align-items: center;
}
.nb4 {
  display: flex;
  align-items: flex-start;
  gap: 5px;
}
.nb5 {
  display: flex;
  width: 450px; /* Adjust the width to make it thinner */
  height: 50px;
  align-items: center;
  border-radius: 50px;
  background: #fff;
  color: rgba(41, 44, 48, 0.5);
  font-family: Poppins;
  font-size: 18px;
  font-style: normal;
  font-weight: 500;
  line-height: normal;
}

.logo {
  font-size: 1.5rem;
  font-weight: bold;
}

.nav-list {
  list-style: none;
  display: flex;
}

.nav-list li {
  margin-right: 20px;
  cursor: pointer;
}
.imagecontainer_image {
  max-height: 50%;
  max-width: 50%;
}
</style>
