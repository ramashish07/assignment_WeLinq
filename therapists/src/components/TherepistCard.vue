<!-- src/components/TherapistCard.vue -->

<template>
  <div class="therapist-card">
    <img class="ellipse" :src="therapist.photoUrl" />
    <div class="overlap-group">
      <div class="text-wrapper">${{ therapist.hourlyRate }}/hr</div>
    </div>
    <div class="frame">
      <div class="div">{{ therapist.nickname }}</div>
      <img class="image" src="../assets/tick.png" />
    </div>
    <div class="text-wrapper-2">Last active 10min ago</div>
    <div class="frame-2">
      <div class="frame-3">
        <img class="solid-award" src="../assets/exp.png" />
        <div class="text-wrapper-3">
          {{ therapist.expertExperience }} year of experience
        </div>
      </div>
      <div class="frame-4">
        <!-- <div class="group"></div> -->

        <img class="fi-sr-graduation-cap" src="../assets/dep.png" />
        <div class="text-wrapper-3">
          {{ therapist.expertFocusArea[0] }},{{ therapist.expertFocusArea[1] }}
        </div>
      </div>
      <div class="frame-5">
        <img class="fi-sr-graduation-cap" src="../assets/beh.png" />
        <div class="text-wrapper-4">{{ therapist.qualification }}</div>
      </div>
    </div>
    <div class="frame-6">
      <div class="div-wrapper">
        <div class="text-wrapper-5">Book session</div>
      </div>
      <div class="fi-rr-comment-wrapper">
        <img
          class="fi-rr-comment"
          src="../assets/chat.png"
          style="height: 30px; width: 35px:"
        />
      </div>
    </div>
  </div>
</template>

<script>
export default {
  props: {
    therapist: {
      type: Object,
      required: true,
    },
  },
  mounted() {
    const focusAreas = this.therapist.expertFocusArea;
    const focusAreasString = focusAreas.join(", ");
    console.log("Focus Areas String:", focusAreasString);
  },
};
</script>

<style scoped>
.therapist-card {
  display: flex;
  position: relative;
  width: 300px;
  height: 250px;
  background-color: #ffffff;
  border-radius: 10px;
  overflow: hidden;
  display: flex;
  flex-direction: column;
}

/* ... (other styles) ... */

.therapist-card .ellipse {
  /* display: flex; */
  position: absolute;
  width: 52px; /* Adjusted width */
  height: 52px; /* Adjusted height */
  top: 8px;
  left: 110px;
  border-radius: 50%;
  justify-content: center;
  align-items: center;
  object-fit: cover;
}

/* ... (other styles) ... */

.therapist-card .overlap-group {
  position: absolute;
  width: 40px;
  height: 20px;
  top: 60px; /* Adjusted top position */
  left: 106px; /* Adjusted left position */
}

/* ... (other styles) ... */

.therapist-card .text-wrapper {
  position: absolute;
  width: 60px; /* Adjusted width */
  top: 0;
  left: 0;
  font-family: "Poppins-SemiBold", Helvetica;
  font-weight: 600;
  color: orange;
  font-size: 14px; /* Adjusted font size */
  text-align: center;
  letter-spacing: -0.25px;
  line-height: 18px; /* Adjusted line height */
}

/* ... (other styles) ... */

.therapist-card .frame {
  display: inline-flex;
  align-items: center;
  gap: 5px; /* Adjusted gap */
  position: absolute;
  top: 75px; /* Adjusted top position */
  left: 80px; /* Adjusted left position */
  color: #292c30;
  font-family: Poppins;
  font-size: 16px;
  font-style: normal;
  font-weight: 600;
  line-height: 24px; /* 133.333% */
  letter-spacing: -0.5px;
}

/* ... (other styles) ... */

.therapist-card .text-wrapper-2 {
  position: absolute;
  top: 95px; /* Adjusted top position */
  left: 80px; /* Adjusted left position */
  font-family: "Poppins-Medium", Helvetica;
  font-weight: 500;
  color: #396ce8;
  font-size: 10px; /* Adjusted font size */
  letter-spacing: -0.25px;
  line-height: normal;
}

/* ... (other styles) ... */

.therapist-card .frame-2 {
  display: inline-flex;
  flex-direction: column;
  align-items: flex-start;
  justify-content: center;
  gap: 2px; /* Adjusted gap */
  position: absolute;

  top: 110px; /* Adjusted top position */
  left: 10px; /* Adjusted left position */
}

.therapist-card .text-wrapper-3 {
  color: #292220;
  font-family: Poppins;
  font-size: 14px;
  font-style: normal;
  font-weight: 500;
  line-height: 131%;
}
.therapist-card .text-wrapper-4 {
  color: #292220;
  font-family: Poppins;
  font-size: 14px;
  font-style: normal;
  font-weight: 500;
  line-height: 131%; /* 18.34px */
}
/* ... (other styles) ... */

.therapist-card .frame-3 {
  display: inline-flex;
  align-items: flex-start;
  gap: 5px; /* Adjusted gap */
  position: relative;
  flex: 0 0 auto;
}

/* ... (other styles) ... */

.therapist-card .frame-4 {
  display: inline-flex;
  align-items: flex-start;
  gap: 3px;
  position: relative;
  flex: 0 0 auto;
}

/* ... (other styles) ... */

.therapist-card .frame-5 {
  display: inline-flex;
  align-items: flex-start;
  gap: 3px; /* Adjusted gap */

  position: relative;
  flex: 0 0 auto;
}

/* ... (other styles) ... */

.therapist-card .frame-6 {
  display: inline-flex;
  align-items: center;
  gap: 8px; /* Adjusted gap */
  position: absolute;
  top: 140px; /* Adjusted top position */
  left: 10px; /* Adjusted left position */
}

/* ... (other styles) ... */

.therapist-card .div-wrapper {
  display: inline-flex;
  margin-top: 35px;
  margin-left: 30px;
  align-items: center;
  gap: 5px; /* Adjusted gap */
  padding: 6px 12px; /* Adjusted padding */
  position: relative;
  flex: 0 0 auto;
  background-color: #e5e7ff;
  border-radius: 5px; /* Adjusted border-radius */
}

/* ... (other styles) ... */

.therapist-card .fi-rr-comment-wrapper {
  position: relative;
  width: 5px; /* Adjusted width */
  height: 5px; /* Adjusted height */
  margin-top: 25px;
  /* background-color: #ccf4da; */
  border-radius: 15px; /* Adjusted border-radius */
}
</style>
