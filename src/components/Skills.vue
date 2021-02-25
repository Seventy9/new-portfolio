<template>
  <div id="skills">
    <h2 id="skills-title">My skills</h2>
    <div id="skills-sysadmin" class="skills-left">
      <i class="fas fa-server fa-5x skills-item-image-left"></i>
      <div class="skills-item-left">
        <h3 class="skills-item-title-left">Systems Administration</h3>
        <p class="skills-item-description">
          For several years I have worked as a Systems Administrator for hosting
          companies and managed service providers. I am comfortable working with
          and supporting all varients of Windows (desktop and server) and Linux
          servers based on Debian and Red Hat Enterprise Linux. I have
          researched, planned completed many projects involving server
          installations, upgrades, and and decommissions and network
          installations and expansions.
        </p>
      </div>
    </div>
    <div id="skills-webdev" class="skills-right">
      <i class="far fa-file-code fa-5x skills-item-image-right"></i>
      <div class="skills-item-right">
        <h3 class="skills-item-title-right">Web Development</h3>
        <p class="skills-item-description">
          I have completed the HTML and CSS chapters of the courses I am
          studying with
          <a
            href="https://www.udemy.com/course/the-complete-web-development-bootcamp/"
            >Udemy</a
          >
          and <a href="https://www.freecodecamp.org/">freeCodeCamp</a>.
          Completing the 5 different projects on freeCodeCamp and gaining the
          <a
            href="https://www.freecodecamp.org/certification/seventy9/responsive-web-design"
            >Responsive Web Development</a
          >
          certificate has given me a good understanding of HTML and CSS which I
          am now able to put into practice in this site. The next part of my
          coding journey is with JavaScript, of which I currently have very
          little knowledge.
        </p>
      </div>
    </div>
    <div id="skills-photography" class="skills-left">
      <i class="far fa-images fa-5x skills-item-image-left"></i>
      <div class="skills-item-left">
        <h3 class="skills-item-title-left">Photography</h3>
        <p class="skills-item-description">
          I enjoy photography in my spare time. I have a Pentax K-50 with a
          18-55mm F3.5-5.6 lens and a 55-300mm F1.4-5.8 telephoto lens. My
          favourite styles of photography are architectural, sports (car and
          motorcycle racing) and portrait. When I am able to I will create a
          gallery website from scratch to share my photographs.
        </p>
      </div>
    </div>
  </div>
</template>

<style lang="scss">
#skills {
  align-items: center;
  display: flex;
  flex-direction: column;
  justify-content: center;
  padding: 10rem 2rem 5rem;
}

#skills a {
  color: var(--highlight-dark);
}

#skills-title {
  margin-bottom: 10rem;
}

.skills-left {
  display: flex;
  margin-bottom: 5rem;
  max-width: 80rem;
}

.skills-right {
  display: flex;
  flex-direction: row-reverse;
  margin-bottom: 5rem;
  max-width: 80rem;
}

.skills-item-left {
  display: flex;
  flex-direction: column;
  text-align: justify;
}

.skills-item-right {
  display: flex;
  flex-direction: column;
  text-align: justify;
}

.skills-item-image-left {
  color: var(--highlight-dark);
  margin-right: 2rem;
  transition: 0.3s;
}

.skills-item-image-right {
  color: var(--highlight-dark);
  margin-left: 2rem;
  transition: 0.3s;
}

.skills-item-title-left {
  padding-bottom: 2rem;
  text-align: left;
}

.skills-item-title-right {
  padding-bottom: 2rem;
  text-align: right;
}

.skills-item-description {
  line-height: 2.4rem;
}

@media (max-width: 768px) {
  .skills-left {
    flex-direction: column;
  }
  .skills-right {
    flex-direction: column;
  }
  .skills-item-image-left {
    padding-bottom: 2rem;
    margin-right: 0;
    text-align: center;
  }
  .skills-item-image-right {
    padding-bottom: 2rem;
    margin-left: 0;
    text-align: center;
  }
  .skills-item-title-left {
    text-align: center;
  }
  .skills-item-title-right {
    text-align: center;
  }
}
</style>
