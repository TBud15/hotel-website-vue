<template>
  <div class="video-container">
    <video autoplay muted loop class="background-video">
      <source src="@/assets/video/vide.mp4" type="video/mp4" />
      Your browser does not support the video tag.
    </video>

    <div class="dark-overlay"></div>

    <div class="content-overlay">
      <div class="top-text">
        <h1 class="main-title">See you soon —</h1>
        <h2 class="subtitle">We will be waiting for you.</h2>
      </div>

      <div class="contact-info">
        <p>Sunfolk Valley</p>
        <p>+123-456-7890</p>
        <p>info@realestatevillas.com</p>
      </div>

      <div class="bottom-box">
        <div class="social-icons">
          <img src="@/assets/social/facebook.png" alt="Facebook" />
          <img src="@/assets/social/instagram.png" alt="Instagram" />
          <img src="@/assets/social/whatsapp.png" alt="WhatsApp" />
        </div>
        <div class="company-name">
          <p>Fairhill Villas</p>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'BackgroundVideoWithDarkOverlay',
}
</script>

<style scoped>
.video-container {
  position: relative;
  width: 100%;
  height: 100vh;
  overflow: hidden;
  color: white;
  display: flex;
  justify-content: center;
  align-items: center;
}

.background-video {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  object-fit: cover;
  z-index: -2;
}

.dark-overlay {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  background-color: rgba(0, 0, 0, 0.3);
  z-index: -1;
}

.content-overlay {
  position: relative;
  width: 90%;
  /* max-width: 1200px; */
  display: flex;
  flex-direction: column;
  justify-content: space-between;
  height: 90%;
}

.top-text {
  margin-bottom: 2rem;
  text-align: left;
  font-family: 'GeorgiaProCond';
}

.top-text h1 {
  font-size: 3.5rem;
  margin: 0;
}

.top-text h2 {
  font-size: 4.5rem;
  margin: 0;
  font-weight: bold;
}

.contact-info {
  margin-top: 1rem;
  font-size: 1.5rem;
  line-height: 2rem;
  text-align: left;
  font-family: 'DMSansRegular';
}

.bottom-box {
  display: flex;
  justify-content: space-between;
  align-items: center;
  margin-top: 2rem;
}

.social-icons img {
  margin-right: 1rem;
  width: 2rem;
  height: auto;
}

.company-name {
  font-size: 6rem;
  font-weight: bold;
  text-align: right;
  font-family: 'EdwardFont';
  max-width: 15rem;
}

/* Responsive Design */
/* mp4 background video might be too long for current responsive design */
@media (max-width: 768px) {
  .top-text h1 {
    font-size: 2.5rem;
  }

  .top-text h2 {
    font-size: 3rem;
  }

  .contact-info {
    font-size: 1.2rem;
  }

  .social-icons img {
    width: 2.5rem;
  }

  .company-name {
    font-size: 1.2rem;
  }
}

@media (max-width: 480px) {
  .content-overlay {
    width: 95%;
  }

  .top-text h1 {
    font-size: 2rem;
  }

  .top-text h2 {
    font-size: 2.5rem;
  }

  .contact-info {
    font-size: 1rem;
  }

  .social-icons img {
    width: 2rem;
  }

  .company-name {
    font-size: 1rem;
  }
}
</style>
