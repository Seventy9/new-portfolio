<template>
  <div id="projects">
    <h2 id="projects-header">Projects (coming soon)</h2>
    <!-- <div id="projects-grid">
          <article class="projects-card">
            <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.</p>
          </article>
          <article class="projects-card">
            <p>Ipsum dolor sit amet consectetur adipiscing elit duis tristique sollicitudin.</p>
          </article>
          <article class="projects-card">
            <p>Elementum facilisis leo vel fringilla est.</p>
          </article>
          <article class="projects-card">
            <p>Egestas maecenas pharetra convallis posuere.</p>
          </article>
          <article class="projects-card">
            <p> Tempor orci dapibus ultrices in iaculis nunc sed.</p>
          </article>
        </div> -->
    <i id="projects-coming-soon" class="fas fa-spinner fa-10x"></i>
  </div>
</template>

<style lang="scss">
#projects {
  background-color: var(--main-grey);
  color: var(--main-white);
  padding: 10rem 2rem;
  text-align: center;
}

#projects-header {
  margin: 0 auto 5rem auto;
  max-width: 64rem;
}

#projects-grid {
  display: grid;
  gap: 5rem;
  grid-template-columns: repeat(auto-fit, minmax(40rem, 1fr));
  margin: 0 auto;
  max-width: 64rem;
  width: 100%;
}

.projects-card {
  background-color: var(--main-blue);
  border: 0.2rem solid #fbd46d;
  height: 40rem;
  padding: 2rem;
}

#projects-coming-soon {
  animation: rotation 2s infinite linear;
  color: var(--main-yellow);
  transition: 0.3s;
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
