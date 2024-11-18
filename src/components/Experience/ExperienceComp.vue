<template>
  <div class="sectiontwo">
    <h1 class="title">Experience a serene retreat surrounded by nature and grandeur</h1>
    <div class="icons">
      <img src="@/assets/website-icons/palm-tree.png" alt="Palm Tree" />
      <img src="@/assets/website-icons/center-left-house.png" alt="Villa One" />
      <img
        src="@/assets/website-icons/center-house.png"
        alt="Villa Two"
        class="villa-center-house"
      />
      <img src="@/assets/website-icons/center-right-house.png" alt="Villa Three" />
      <img src="@/assets/website-icons/palm-tree.png" alt="Palm Tree" />
    </div>
    <p class="paragraph">
      What's special about your product, service, or company? Use this space to highlight the things
      that set you apart from your competition, whether it's a special feature, a unique philosophy,
      or awards and recognition that you have received. Think of this as your elevator pitch to get
      the reader's attention.
    </p>
  </div>
</template>

<style>
.sectiontwo {
  background-color: #642b62;
  padding-top: 1px;
}

.title {
  text-align: center;
  margin-top: 4rem;
  color: white;
  font-family: 'GeorgiaProCond';
}

.icons {
  display: flex;
  justify-content: center;
  gap: 2rem;
  flex-wrap: wrap;
}

.icons img {
  height: 10rem;
  margin-top: 3rem;
  margin-bottom: 3rem;
}

.villa-center-house {
  height: 13rem !important;
}

.paragraph {
  font-family: 'Geist';
  color: white;
  width: 80rem;
  font-size: 1.5rem;
  margin: 0 auto;
  text-align: center;
  padding-bottom: 4rem;
}

/* responsive styling section start */
@media (max-width: 1024px) {
  .paragraph {
    width: 90%;
    font-size: 1.2rem;
  }

  .icons img {
    height: 5rem;
  }

  .villa-center-house {
    height: 7rem !important;
  }
}

@media (max-width: 768px) {
  .icons {
    gap: 1rem;
  }

  .icons img {
    height: 4rem;
  }

  .villa-center-house {
    height: 5rem !important;
  }

  .title {
    font-size: 1.8rem;
    margin-top: 2rem;
  }

  .paragraph {
    font-size: 1rem;
    line-height: 1.5;
  }
}

@media (max-width: 480px) {
  .icons img {
    height: 3rem;
  }

  .villa-center-house {
    height: 2rem !important;
  }

  .title {
    font-size: 1.5rem;
    margin-top: 1.5rem;
  }

  .paragraph {
    font-size: 0.9rem;
  }
}
</style>
