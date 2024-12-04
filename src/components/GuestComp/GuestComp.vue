<template>
  <div class="component">
    <h1 class="title">What Our Guests Say About Us</h1>

    <div class="wrapper">
      <div class="box">
        <img src="@/assets/other/line2.png" alt="Divider Line" />
        <p>
          "Boost your product and service's credibility by adding testimonials from your clients.
          People love recommendations so feedback from others who've tried it is invaluable."
        </p>
        <p class="client-name">Larisa Varma</p>
      </div>
      <div class="box">
        <img src="@/assets/other/line2.png" alt="Divider Line" />
        <p>
          "Boost your product and service's credibility by adding testimonials from your clients.
          People love recommendations so feedback from others who've tried it is invaluable."
        </p>
        <p class="client-name">Gaja Dubicki</p>
      </div>
      <div class="box">
        <img src="@/assets/other/line2.png" alt="Divider Line" />
        <p>
          "Boost your product and service's credibility by adding testimonials from your clients.
          People love recommendations so feedback from others who've tried it is invaluable."
        </p>
        <p class="client-name">Posha Chopra</p>
      </div>
    </div>
  </div>
</template>

<style scoped>
.component {
  background-color: #642b62;
  color: white;
  padding-bottom: 4rem;
}

.wrapper {
  display: flex;
  justify-content: center;
  gap: 5rem;
}

.title {
  text-align: center;
  padding-top: 2rem;
  padding-bottom: 2rem;
}

.box {
  max-width: 30rem;
}

.box p {
  margin-bottom: 1rem;
  font-family: 'DMSansRegular';
  font-size: 1.25rem;
}

.box img {
  max-width: 5rem;
}

.box .client-name {
  font-family: 'EdwardianFont';
  font-size: 2.5rem;
}

@media (max-width: 768px) {
  .wrapper {
    flex-direction: column;
    align-items: center;
    gap: 2rem;
  }

  .box {
    max-width: 90%;
  }

  .box p {
    font-size: 1.1rem;
  }

  .box .client-name {
    font-size: 2rem;
  }
}

@media (max-width: 480px) {
  .title {
    font-size: 1.5rem;
    padding-top: 1rem;
    padding-bottom: 1rem;
  }

  .box {
    max-width: 100%;
  }

  .box p {
    font-size: 1rem;
  }

  .box .client-name {
    font-size: 1.75rem;
  }
}
</style>
