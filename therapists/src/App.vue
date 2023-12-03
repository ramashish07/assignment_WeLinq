<!-- src/App.vue -->
<template>
  <div id="app">
    <div id="main_screen">
      <SideNavigation />
      <div id="main_content">
        <Navbar />
        <div id="main_container">
          <div id="middle_section">
            <div id="categories">
              <div class="filtor" style="background: black; color: white">
                <img src="./assets/tag.png" style="margin-right: 5px" /> Tags
              </div>
              <div class="filtor">Depression</div>
              <div class="filtor">Relationship</div>
              <div class="filtor">Social anxiety</div>
              <div class="filtor">Social anxiety</div>
              <div class="filtor">Social anxiety</div>
              <div class="filtor">Social anxiety</div>
              <div class="filtor">Fighting</div>
            </div>
            <div id="grid_here">
              <div id="therepists-grid">
                <TherepistCard
                  v-for="therapist in therapists"
                  :key="therapist.id"
                  :therapist="therapist"
                />
              </div>
            </div>
          </div>
          <RightSidebar />
        </div>
      </div>
    </div>
    <FooterSection />
  </div>
</template>

<script>
import axios from "axios";
import FooterSection from "./components/FooterSection.vue";
import SideNavigation from "./components/SideNavigation.vue";
import Navbar from "./components/NavbarSection.vue";
import RightSidebar from "./components/RightSidebar.vue";
import TherepistCard from "./components/TherepistCard.vue";

export default {
  name: "App",
  components: {
    FooterSection,
    SideNavigation,
    Navbar,
    RightSidebar,
    TherepistCard,
  },
  data() {
    return {
      therapists: [],
    };
  },
  mounted() {
    // Make API request when the component is mounted
    this.fetchTherapists();
  },
  methods: {
    async fetchTherapists() {
      try {
        // Make API request to fetch therapists
        const response = await axios.get(
          "https://api-container-ph3rhhnyiq-uc.a.run.app/therapists"
        );

        // Update therapists data with the response
        this.therapists = response.data;
      } catch (error) {
        console.error("Error fetching therapists:", error.message);
      }
    },
  },
};
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  text-align: center;
  color: #2c3e50;
  margin: 0;
  padding: 0;
  display: flex;
  flex-direction: column;
  width: 100vw;
  min-height: 100vh;
  overflow-x: hidden;
}

#grid_here {
  display: flex;
  flex-wrap: wrap;
  justify-content: space-around;
  padding: 20px;
}
main {
  border: 5px solid #868cd1;
  flex: 1;
  background: #f4f5ff;
}
.content-column {
  flex: 1;
}
.filtor {
  display: flex;
  height: 30px;
  width: 400px;
  border-radius: 5px;
  background: #fff;
  color: #292c30;
  font-family: Poppins;
  font-size: 12px;
  font-style: normal;
  font-weight: 400;
  line-height: 131%; /* 15.72px */
  align-items: center;
  justify-content: center;
}

#main_screen {
  display: flex;
  height: 100%;
  width: 100%;
}
#main_content {
  display: flex;
  flex-direction: column;
  background: #f4f5ff;
  align-items: stretch;
  /* width: 200px; */
  /* max-width: 100%; */
}
#main_container {
  padding-left: 24px;
  display: flex;
  gap: 24px;
}
#categories {
  display: flex;
  padding: 10px;
  align-items: flex-start;
  gap: 30px;
  border-radius: 5px;
  margin-left: 40 px;
  /* margin-right: 10px; */
}
Navbar {
  flex: 1;
}
SideNavigation {
  flex: 1;
}
#carts {
  width: 267px;
  height: 316px;
  border-radius: 10px;
  background: #fff;
}
#middle_section {
  width: 60vw;
}
#therepists-grid {
  display: grid;
  grid-template-columns: repeat(3, 1fr); /* Create 3 equal columns */
  column-gap: 16px; /* Add gap between cards */
  row-gap: 16px; /* Add gap between cards */
}
</style>
