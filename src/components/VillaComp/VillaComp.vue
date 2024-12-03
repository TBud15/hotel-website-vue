<template>
  <div class="wrapper">
    <div class="left-box">
      <h1>Garden Villa</h1>
      <img src="@/assets/other/line.png" alt="Divider Line" class="divider-line" />
      <p>
        Showcase the best your property has to offer by highlighting one of your accommodations. Add
        a flattering photo, then describe the room's best feature.
      </p>
    </div>
    <div class="image-box"></div>
  </div>
</template>

<style scoped>
.wrapper {
  display: flex;
  align-items: center;
  height: 100vh;
  margin-top: 2rem;
}

.left-box {
  flex: 1;
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  padding: 20px;
  text-align: center;
}

.left-box img {
  size: 2rem;
}

.left-box h1 {
  font-family: 'GeorgiaProCond';
  color: #7b2543;
  font-size: 4rem;
}

.left-box p {
  font-family: 'DMSansRegular';
  max-width: 30rem;
  color: #7b2543;
  font-size: 1.5rem;
}

.divider-line {
  width: 12rem;
  height: auto;
}

.image-box {
  flex: 1;
  background-image: url('@/assets/villas/first-image.jpg');
  background-size: cover;
  background-position: bottom;
  height: 100%;
}
</style>
