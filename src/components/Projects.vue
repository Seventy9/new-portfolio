<template>
  <div id="projects">
    <h2 id="projects-header">Projects</h2>
    <div id="projects-grid">
      <div class="projects-card">
        <div class="projects-class-image"></div>
        <p class="projects-card-description">
          Lorem ipsum dolor sit amet consectetur, adipisicing elit.
        </p>
      </div>
      <div class="projects-card">
        <img class="projects-card-image" src="../assets/images/2.jpg" />
        <p class="projects-card-description">
          Quis reiciendis magnam dolorem sit fugiat.
        </p>
      </div>
      <div class="projects-card">
        <img class="projects-card-image" src="../assets/images/3.jpg" />
        <p class="projects-card-description">
          Elementum facilisis leo vel fringilla est.
        </p>
      </div>
      <div class="projects-card">
        <img class="projects-card-image" src="../assets/images/4.jpg" />
        <p class="projects-card-description">
          Egestas maecenas pharetra convallis posuere.
        </p>
      </div>
      <div class="projects-card">
        <img class="projects-card-image" src="../assets/images/5.jpg" />
        <p class="projects-card-description">
          Tempor orci dapibus ultrices in iaculis nunc sed.
        </p>
      </div>
      <div class="projects-card">
        <img class="projects-card-image" src="../assets/images/6.jpg" />
        <p class="projects-card-description">
          Lorem ipsum dolor sit amet, consectetur adipisicing elit.
        </p>
      </div>
    </div>
  </div>
</template>

<style lang="scss">
#projects {
  background-color: var(--background-dark);
  color: var(--text-light);
  padding: 10rem 2rem;
  text-align: center;
}

#projects-header {
  margin: 0 auto 5rem auto;
  max-width: 64rem;
}

#projects-grid {
  display: grid;
  gap: 1rem;
  grid-template-columns: repeat(3, 25rem);
  grid-template-rows: repeat(2, 35rem);
  margin: 0 auto;
  max-width: 80rem;
  width: 100%;
}

.projects-card {
  background-color: var(--background-light);
  color: var(--text-dark);
  border: 0.2rem solid var(--highlight-light);
  padding: 2rem;
}

.projects-card-image {
  background-image: url("../assets/images/1.jpg");
  background-position: center;
  background-size: cover;
  height: 20rem;
  overflow: hidden;
}

.projects-card-description {
  line-height: 2.4rem;
}

@keyframes rotation {
  from {
    transform: rotate(0deg);
  }
  to {
    transform: rotate(359deg);
  }
}
</style>
