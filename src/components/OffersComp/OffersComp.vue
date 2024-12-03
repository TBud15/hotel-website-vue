<template>
  <h1 class="title">Special Offers</h1>
  <div class="wrapper">
    <div class="box">
      <img src="@/assets/website-icons/flower.png" alt="Flowers" />
      <h3>Summer to Remember</h3>
      <p>
        List your offers, promos, or special membership privileges and perks here to entice people
        to book your property.
      </p>
    </div>
    <div class="box">
      <img src="@/assets/website-icons/champ.png" alt="Champagne" />
      <h3>Wine and Dine</h3>
      <p>
        List your offers, promos, or special membership privileges and perks here to entice people
        to book your property.
      </p>
    </div>
    <div class="box">
      <img src="@/assets/website-icons/box.png" alt="Box" />
      <h3>Weekend Wanderlust</h3>
      <p>
        List your offers, promos, or special membership privileges and perks here to entice people
        to book your property.
      </p>
    </div>
  </div>
</template>

<style scoped>
.title {
  font-family: 'GeistRegular';
  text-align: center;
  color: #642b62;
  margin-top: 1rem;
  margin-bottom: 2rem;
  font-size: 3rem;
}

.wrapper {
  display: flex;
  justify-content: center;
  gap: 10rem;
  padding-bottom: 4rem;
}

.box {
  max-width: 20rem;
  text-align: center;
}

.box p {
  color: #642b62;
  font-family: 'DMSansRegular';
  font-size: 1.25rem;
}

.box h3 {
  color: #642b62;
  margin-top: 1rem;
  margin-bottom: 1rem;
}

.box img {
  max-width: 20rem;
  max-height: 15rem;
}

@media (max-width: 1024px) {
  .title {
    margin-bottom: 2rem;
  }

  .wrapper {
    flex-direction: column;
    align-items: center;
    gap: 2rem;
  }
}
</style>
