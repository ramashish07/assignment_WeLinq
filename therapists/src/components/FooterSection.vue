<template>
  <footer>
    <div class="frame">
      <div class="frame_2">
        <div class="frame_3">
          <div style="width: 60px; height: 60px">
            <img
              src="../assets/footer_preview.png"
              alt="image not loaded"
              style="max-width: 100%; max-height: 100%; display: block"
            />
          </div>
          <div>
            <div class="head">Product</div>
            <div class="subcontent">Affiliate Program</div>
          </div>
          <div>
            <div class="head">Resources</div>
            <div class="subcontent">Blog</div>
            <div class="subcontent">Become Therapists</div>
            <div class="subcontent">Apply for Therapists</div>
          </div>
          <div>
            <div class="head">Useful Links</div>
            <div class="subcontent">Terms</div>
            <div class="subcontent">Privacy Policy</div>
          </div>
          <div>
            <div class="head">Flow us on</div>
            <div class="subcontent">
              <img
                src="../assets/fb_logo.png"
                alt="Facebook Logo"
                style="height: 15px; width: 15px"
              />
              Facebook
            </div>
            <div class="subcontent">
              <img
                src="../assets/linkedin.png"
                alt="Facebook Logo"
                style="height: 15px; width: 15px"
              />
              Linedin
            </div>
            <div class="subcontent">
              <img
                src="../assets/twitter.png"
                alt="Facebook Logo"
                style="height: 15px; width: 15px"
              />
              Twitter
            </div>
            <div class="subcontent">
              <img
                src="../assets/insta.png"
                alt="Facebook Logo"
                style="height: 15px; width: 15px"
              />
              Instagram
            </div>
          </div>
        </div>
        <div class="frame_6">
          <img class="vector" src="../assets/Vector80.png" />
          <p class="p">© 2023 Einstein Limited. All rights reserved.</p>
        </div>
      </div>
    </div>
  </footer>
</template>

<script>
export default {
  // You can add component-specific logic here if needed
};
</script>

<style scoped>
/* Add styling for the footer here */
footer {
  /* position: fixed; */
  width: 100vw;
  height: 30vh;
  justify-content: center;
  align-items: center;
  flex-shrink: 0;
  background: #eeefff;
  display: flex;
  z-index: 999; /* Adjust the z-index as needed */
}

.frame {
  display: flex;
  align-items: start;
  justify-items: start;
  gap: 30px;
}
.frame_2 {
  display: flex;
  flex-direction: column;
  align-items: center;
  gap: 20px;
}
.frame_3 {
  display: flex;
  align-items: flex-start;
  gap: 100px;
}
.footer_img {
  display: flex;
  /* height: 60px; */
  /* width: 60px; */
  /* justify-content: center;
  align-items: center; */
  padding: 5px 25px 0px 0px;
  /* border-radius: 50%; */
  background: #868cd1;
}
.head {
  display: flex;
  color: #292c30;
  font-family: Poppins;
  font-size: 20px;
  font-style: normal;
  font-weight: 500;
  line-height: normal;
}
.subcontent {
  display: flex;
  color: #292c30;
  font-family: Poppins;
  font-size: 14px;
  font-style: normal;
  font-weight: 400;
  line-height: normal;
  margin-top: 5px;
}
.media_icon {
  height: 15px;
  width: 15px;
}
/* .frame > div {
  display: flex;
  flex-direction: column;
  gap: 4px;
  align-items: left;
  justify-content: start;
} */
/* .frame > div > h4 {
  margin-bottom: 4px;
  font-size: 24px;
  text-align: left;
  margin: 0;
}
.frame > div > p {
  font-size: 16px;
  text-align: left;
}
.frame > .footer_img {
  height: 100px;
  width: 100px;
  padding-right: 50px;
  margin-right: auto;
}
.frame > .footer_img > img {
  height: 100%;
  width: 100%;
} */
</style>
