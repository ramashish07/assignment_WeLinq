<!-- src/components/RightSidebar.vue -->

<template>
  <div class="right-sidebar">
    <div class="rs1">
      <img src="../assets/propic.svg" alt="image not loaded" class="profile" />
      <div class="rs1_inside">
        <div class="text"><b> Sneha ai</b></div>
        <div class="text2">Anxiety,Depression Specialist</div>
        <div class="profile_button">View profile</div>
      </div>
    </div>
    <div class="rs2">
      <div class="calendar">
        <div class="month_selectors">
          <div class="select_month">
            <p>{{ "<" }}</p>
            <p>August ▼</p>
            <p>{{ ">" }}</p>
          </div>
          <div class="select_year">
            <p>{{ "<" }}</p>
            <p>2023 ▼</p>
            <p>{{ ">" }}</p>
          </div>
        </div>
        <div class="calendar_main">
          <div class="weeknames">
            <p>Mon</p>
            <p>Tue</p>
            <p>Wed</p>
            <p>Thu</p>
            <p>Fri</p>
            <p>Sat</p>
            <p>Sun</p>
          </div>
          <div class="dates">
            <p class="prev_month">28</p>
            <p class="prev_month">29</p>
            <p class="prev_month">30</p>
            <p class="prev_month">31</p>
            <p>1</p>
            <p>2</p>
            <p>3</p>
            <p>4</p>
            <p>5</p>
            <p>6</p>
            <p>7</p>
            <p>8</p>
            <p>9</p>
            <p>10</p>
            <p class="available_date">11</p>
            <p class="available_date">12</p>
            <p class="available_date">13</p>
            <p class="available_date">14</p>
            <p class="available_date">15</p>
            <p>16</p>
            <p>17</p>
            <p>18</p>
            <p class="available_date">19</p>
            <p class="available_date">20</p>
            <p class="available_date">21</p>
            <p class="available_date">22</p>
            <p>23</p>
            <p>24</p>
            <p>25</p>
            <p>26</p>
            <p>27</p>
            <p class="available_date">28</p>
            <p class="available_date">29</p>
            <p>30</p>
            <p>31</p>
            <p class="nex_month">1</p>
            <p class="nex_month">2</p>
            <p class="nex_month">3</p>
            <p class="nex_month">4</p>
            <p class="nex_month">5</p>
            <p class="nex_month">6</p>
            <p class="nex_month">7</p>
          </div>
        </div>
      </div>
    </div>

    <div class="rs3">
      <div class="section_heading">Session Period</div>
      <div class="time_selector">60 min</div>
      <p class="sub_text">Note: *session period will be of 60min</p>
    </div>

    <div class="rs4">
      <div class="section_heading">Session Time</div>
      <div class="time_selector">
        <div class="time_am">
          <p class="time_dot">.</p>
          <p class="time_name">AM</p>
        </div>
        <div class="time_pm">
          <p class="time_dot">.</p>
          <p class="time_name">PM</p>
        </div>
      </div>
      <div class="slots">
        <p>10:00 AM</p>
        <p>11:00 AM</p>
        <p class="slot_selected">12:00 AM</p>
        <p>10:30 AM</p>
        <p>11:30 AM</p>
        <p>12:30 AM</p>
      </div>
    </div>
    <div class="rs5">
      <div class="book">Book session</div>
    </div>
  </div>
</template>

<script>
export default {
  // You can add component-specific logic here if needed
};
</script>

<style scoped>
/* Add styling for the right sidebar here */
.right-sidebar {
  width: 20vw;
  max-width: 100%;
  background-color: white;
  padding: 20px;
  display: flex;
  flex-direction: column;
  margin-left: 0; /* Push the right sidebar to the rightmost */
  height: 100%;
}

.rs1 {
  display: flex;
  align-items: center;
  gap: 20px;
  border: 2px #868cd1;
  width: 300px;
}
.rs2 {
  display: inline-flex;
  flex-direction: column;
  align-items: center;
  gap: 12px;
  border-radius: 10px;
  border: 1px solid #c0c5fc;
  background: #fff;
  width: 260px;
}
.book {
  color: #fff;
  text-align: center;
  font-family: Poppins;
  font-size: 16px;
  font-style: normal;
  font-weight: 500;
  line-height: 24px; /* 150% */
  letter-spacing: -0.25px;
  justify-content: center;
  align-items: center;
  display: flex;
}
.rs3 {
  display: inline-flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  width: 260px;
  border-radius: 10px;
  border: 1px solid #c0c5fc;
  background: #fff;
}
.rs3 > .section_heading {
  color: #000000;
  font-size: 18px;
  margin-top: 8px;
}
.rs3 > .time_selector {
  color: #000000;
  font-size: 14px;
  padding: 6px 16px;
  border-radius: 4px;
  font-weight: 600;
  background: #e5e7ff;
}
.rs3 > .sub_text {
  font-size: 12px;
  color: grey;
  margin-top: 8px;
}
.rs4 {
  display: inline-flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  width: 260px;
  border-radius: 10px;
  border: 1px solid #c0c5fc;
  background: #fff;
}
.rs4 > .section_heading {
  color: #000000;
  font-size: 18px;
  margin-top: 8px;
}
.rs4 > .time_selector {
  color: #000000;
  font-size: 14px;
  display: flex;
  gap: 16px;
}
.rs4 > .time_selector p {
  margin: 0;
}
.rs4 > .time_selector > div {
  display: flex;
  align-items: center;
  justify-content: center;
  gap: 4px;
}
.rs4 > .time_selector .time_dot {
  height: 8px;
  width: 8px;
  color: transparent;
  border-radius: 50%;
}
.rs4 > .time_selector > .time_am > .time_dot {
  background: #868cd1;
}
.rs4 > .time_selector > .time_pm > .time_dot {
  background: rgb(211, 211, 211);
}
.rs3 > .sub_text {
  font-size: 12px;
  color: grey;
  margin-top: 8px;
}
.rs4 {
  display: inline-flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  width: 260px;
  border-radius: 10px;
  border: 1px solid #c0c5fc;
  background: #fff;
}
.rs4 > .slots {
  display: grid;
  grid-template-columns: auto auto auto;
  column-gap: 2px;
  font-size: 12px;
  align-items: center;
}
.rs4 > .slots > p {
  padding: 4px 12px;
  border-radius: 4px;
}
.rs4 > .slots > .slot_selected {
  background: #e5e7ff;
}
.rs5 {
  display: inline-flex;
  /* padding: 12px 120px; */
  align-items: flex-start;
  gap: 10px;
  border-radius: 10px;
  width: 260px;
  padding: 6px 16px;
  align-items: center;
  justify-content: center;
  background: #868cd1;
}
.right-sidebar div {
  margin-bottom: 10px;
  cursor: pointer;
}
.rs1_inside {
  display: flex;
  flex-direction: column;
  align-items: flex-start;
}
.profile {
  height: 80px;
  width: 80px;
}
.profile_button {
  padding: 4px 16px;
  border-radius: 6px;
  font-size: 14px;
  color: white;
  background: #868cd1;
}
.text {
  color: #292c30;
  font-family: Poppins;
  font-size: 20px;
  font-style: normal;
  font-weight: 500;
  line-height: normal;
  margin: 0;
}
.calendar {
  display: flex;
  flex-direction: column;
}
.text2 {
  color: #292c30;
  font-family: Poppins;
  font-size: 12px;
  font-style: normal;
  font-weight: 400;
  line-height: normal;
  margin: 0;
}

.calendar > .month_selectors {
  display: flex;
  gap: 16px;
  margin-top: 8px;
  font-size: 14px;
}
.calendar > .month_selectors p {
  margin: 0;
}
.calendar > .month_selectors > .select_month,
.calendar > .month_selectors > .select_year {
  display: flex;
  gap: 12px;
}
.calendar_main {
  display: flex;
  flex-direction: column;
  width: 100%;
  font-size: 14px;
}
.calendar_main p {
  padding: 0;
  margin: 0;
}
.calendar_main > .weeknames {
  display: grid;
  grid-template-columns: auto auto auto auto auto auto auto;
  gap: 8px;
  align-items: center;
}
.calendar_main > .dates {
  display: grid;
  grid-template-columns: auto auto auto auto auto auto auto;
  row-gap: 4px;
  column-gap: 0;
}
.calendar_main > .dates > p {
  font-weight: 600;
}
.calendar_main > .dates > .prev_month,
.calendar_main > .dates > .nex_month {
  color: rgba(41, 44, 48, 0.5);
}
.calendar_main > .dates > .available_date {
  background: #e5e7ff;
}
</style>
