<template>
  <div class="wrapper">
    <div class="left-box">
      <img src="@/assets/villas/room/image-one.webp" alt="Room Image" />
      <p>
        An intriguing caption that describes the room goes here. Use a flattering photo, then
        describe away.
      </p>
    </div>
    <div class="right-box">
      <p>
        An intriguing caption that describes the room goes here. Use a flattering photo, then
        describe away.
      </p>
      <img src="@/assets/villas/room/image-two.webp" alt="Couple Image" />
    </div>
  </div>
</template>

<style scoped>
.wrapper {
  display: flex;
  justify-content: space-evenly;
  align-items: flex-start;
  background-color: #b093a8;
  padding: 2rem;
  gap: 2rem;
  flex-wrap: wrap;
}

.left-box,
.right-box {
  display: flex;
  flex-direction: column;
  align-items: center;
  max-width: 30rem;
  flex: 1 1 45%;
  color: white;
}

.left-box img,
.right-box img {
  height: 45rem;
  width: 100%;
  object-fit: cover;
  margin-bottom: 1rem;
}

.left-box p,
.right-box p {
  font-family: 'DMSansRegular';
  text-align: center;
  font-size: 1.2rem;
  line-height: 1.6;
  margin: 0;
  padding: 1rem;
}

@media (max-width: 1024px) {
  .wrapper {
    gap: 1rem;
  }

  .left-box img,
  .right-box img {
    height: 35rem;
  }
}

@media (max-width: 768px) {
  .wrapper {
    flex-direction: column;
    align-items: center;
  }

  .left-box,
  .right-box {
    max-width: 100%;
    flex: none;
  }

  .left-box img,
  .right-box img {
    height: auto;
    width: 100%;
  }

  .left-box p,
  .right-box p {
    font-size: 1rem;
    padding: 0.5rem;
  }
}
</style>
