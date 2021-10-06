<template>
  <div>
    <footer>
      <div class="footer-flex">
        <div class="footer-container">
          <div class="footer-logo">
            <img
              :src="require('~/assets/images/footer-logo.png')"
              class="footer-logo"
            />
          </div>
          <div class="footer-center">
            <div class="footer-links">
              <a href="">SIGN IN</a>
              <a href="">SIGN UP</a>
              <a href="">404</a>
              <a href="">SUPPORT</a>
              <a href="">GET THEME</a>
            </div>
            <div class="copyright-div">
              THINKTECH © 2020 - All rights reserved.
            </div>
          </div>
          <div class="footer-sm">
            <a href=""><i class="fab fa-facebook"></i></a>
            <a href=""><i class="fab fa-whatsapp"></i></a>
            <a href=""><i class="fab fa-twitter"></i></a>
            <a href=""><i class="fab fa-linkedin"></i></a>
          </div>
        </div>
      </div>
    </footer>
  </div>
</template>

<style lang="scss" scoped>
footer {
  text-align: center;
  display: flex;
  align-items: center;
  justify-content: center;
  border-top: 1px solid rgba(66, 66, 65, 0.322);
}

.footer-container {
  display: grid;
  grid-gap: 0.5rem;
  align-items: center;
  max-width: 1200px;
  margin: 0 auto;
  padding-left: 20px;
  padding-right: 20px;
  position: relative;
}

.footer-logo {
  height: 150px;
  width: auto;
  align-items: flex-start;
}

.footer-logo img {
  overflow: hidden;
  object-fit: contain;
}
.footer-links {
  display: block;
  font-size: 13px;
}

.copyright-div {
  font-size: 11px;
  padding: 0;
  margin: 1rem 0 0;
  text-align: center;
}
.footer-links a {
  color: var(--dark);
  padding: 0.25rem;
}

@media screen and (min-width: 768px) {
  .footer-title {
    top: -56%;
    left: 0;
  }
  .footer-container {
    grid-template-columns: repeat(3, 1fr);
  }
  .footer-links {
    display: block;
    white-space: nowrap;
    justify-self: center;
  }
  .footer-container a {
    margin: 0 0.25rem;
  }
  .footer-sm {
    justify-self: flex-end;
  }
}
</style>
