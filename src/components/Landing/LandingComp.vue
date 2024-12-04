<template>
  <div class="hero-section">
    <Transition name="fade-slide">
      <div class="content" v-if="showContent">
        <h4 class="subtitle">SUNFOLK VALLEY</h4>
        <h1 class="title">Fairhill Villas</h1>
        <div>
          <p class="tagline">A Countryside Getaway</p>
          <button class="cta-button">Book Your Stay Now</button>
        </div>
      </div>
    </Transition>
    <div class="frame-image" :style="{ backgroundImage: 'url(' + imageFrameUrl + ')' }"></div>
  </div>
</template>

<script>
import imageFrame from '@/assets/other/image-frame.png'

export default {
  data() {
    return {
      imageUrl: 'https://media-public.canva.com/PLYOw/MAEpYUPLYOw/1/s3.jpg',
      imageFrameUrl: imageFrame,
      showContent: false, // content visibility
    }
  },
  mounted() {
    // show content after delay
    setTimeout(() => {
      this.showContent = true
    }, 200)
  },
}
</script>

<style scoped>
.hero-section {
  position: relative;
  width: 100%;
  height: 100vh;
  background: url('https://media-public.canva.com/PLYOw/MAEpYUPLYOw/1/s3.jpg') no-repeat center
    center/cover;
  display: flex;
  justify-content: center;
  align-items: center;
  color: white;
  font-family: serif;
  box-shadow: 0 0 20px rgba(0, 0, 0, 0.6);
}

.frame-image {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  z-index: 2;
  background-repeat: no-repeat;
  background-position: center center;
  background-size: contain;
  pointer-events: none;
}

.content {
  position: relative;
  z-index: 3;
  text-align: center;
  max-width: 700px;
}

.fade-slide-enter-active,
.fade-slide-leave-active {
  transition:
    opacity 0.5s ease,
    transform 0.5s ease;
}

.fade-slide-enter-from,
.fade-slide-leave-to {
  opacity: 0;
}

.subtitle {
  font-size: 1.5rem;
  letter-spacing: 2px;
  text-transform: uppercase;
  margin-bottom: 10px;
  font-family: 'GeorgiaProCond';
}

.title {
  font-size: 7rem;
  font-family: 'EdwardFont', cursive;
  margin-bottom: 10px;
}

.tagline {
  font-size: 18px;
  font-style: italic;
  margin-bottom: 20px;
  font-family: 'GeorgiaProCond';
}

.cta-button {
  font-size: 1rem;
  font-family: 'GeistRegular';
  padding: 10px 20px;
  border: none;
  background-color: #b093a8;
  color: white;
  cursor: pointer;
  transition: all 0.3s;
}

.cta-button:hover {
  background-color: rgba(255, 255, 255, 0.4);
}

@media (max-width: 768px) {
  .subtitle {
    font-size: 12px;
  }

  .title {
    font-size: 60px;
  }

  .tagline {
    font-size: 14px;
  }

  .cta-button {
    font-size: 12px;
  }
}

@media (max-width: 480px) {
  .subtitle {
    font-size: 10px;
  }

  .title {
    font-size: 45px;
  }

  .tagline {
    font-size: 12px;
  }

  .cta-button {
    font-size: 10px;
    padding: 8px 16px;
  }
}
</style>
