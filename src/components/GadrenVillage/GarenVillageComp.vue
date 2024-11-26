<template>
  <div class="section">
    <p class="title">Villas</p>
    <div class="images-section">
      <div class="villa-card">
        <img src="@/assets/villas/first-image.jpg" alt="Garden Villa" class="image arch" />
        <p class="villa-title">Garden Villa</p>
        <p class="price">Starts at $239/night</p>
        <p class="details">Max 3 Guests</p>
        <p class="details">1 Queen or 2 Twin Beds</p>
      </div>
      <div class="villa-card">
        <img src="@/assets/villas/second-image.jpg" alt="Courtyard Villa" class="image arch" />
        <p class="villa-title">Courtyard Villa</p>
        <p class="price">Starts at $339/night</p>
        <p class="details">Max 5 Guests</p>
        <p class="details">2 Queen or 3 Twin Beds</p>
      </div>
      <div class="villa-card">
        <img src="@/assets/villas/third-image.jpg" alt="Poolside Villa" class="image arch" />
        <p class="villa-title">2-BR Poolside Villa</p>
        <p class="price">Starts at $399/night</p>
        <p class="details">Max 5 Guests</p>
        <p class="details">2 King or 3 Queen Beds</p>
      </div>
    </div>
  </div>
</template>

<style scoped>
.section {
  padding: 2rem;
  text-align: center;
}

.title {
  font-size: 2rem;
  color: #642b62;
  font-family: 'GeorgiaProCond';
  margin-bottom: 2rem;
}

.images-section {
  display: flex;
  justify-content: center;
  gap: 5rem;
}

.villa-card {
  max-width: 300px;
  text-align: center;
}

.image {
  height: 20rem;
  object-fit: cover;
  clip-path: polygon(50% 0%, 100% 38%, 100% 100%, 0 100%, 0% 38%);
}

.arch {
  overflow: hidden;
}

.villa-title {
  font-family: 'DMSansBold';
  font-weight: bold;
  color: #5c2d91;
  margin-top: 1rem;
}

.price {
  font-family: 'DMSansRegular';
  font-size: 1rem;
  color: #5c2d91;
  margin: 0.5rem 0;
}

.details {
  font-family: 'DMSansRegular';
  font-size: 0.9rem;
  color: #333;
}
</style>
