<template>
  <div class="hero-section">
    <div class="content">
      <h4 class="subtitle">SUNFOLK VALLEY</h4>
      <h1 class="title">Fairhill Villas</h1>
      <p class="tagline">A Countryside Getaway</p>
      <button class="cta-button">Book Your Stay Now</button>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      imageUrl: 'https://media-public.canva.com/PLYOw/MAEpYUPLYOw/1/s3.jpg',
    }
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

.hero-section .content {
  text-align: center;
  max-width: 700px;
}

.subtitle {
  font-size: 14px;
  letter-spacing: 2px;
  text-transform: uppercase;
  margin-bottom: 10px;
}

.title {
  font-size: 90px;
  font-family: 'EdwardFont', cursive;
  margin-bottom: 10px;
}

.tagline {
  font-size: 18px;
  font-style: italic;
  margin-bottom: 20px;
}

.cta-button {
  font-size: 14px;
  padding: 10px 20px;
  border: none;
  background-color: rgba(255, 255, 255, 0.2);
  color: white;
  cursor: pointer;
  transition: all 0.3s;
}

.cta-button:hover {
  background-color: rgba(255, 255, 255, 0.4);
}

.hero-section::before {
  content: '';
  position: absolute;
  top: 250px;
  bottom: 250px;
  left: 500px;
  right: 500px;
  border: 1px solid rgba(255, 255, 255, 0.8);
  pointer-events: none;
}
</style>
