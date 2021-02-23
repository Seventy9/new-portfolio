<template>
  <div id="about">
    <img id="about-image" src="../assets/images/me.jpg" alt="Me" />
    <h2 id="about-title">About Me</h2>
    <p id="about-description">
      I am currently learning to become a web developer. I am studying online
      with the course "The Complete 2020 Web Development Bootcamp" by Angela Wu
      on
      <a
        href="https://www.udemy.com/course/the-complete-web-development-bootcamp/"
        >Udemy</a
      >
      and by completing certifications on
      <a href="https://www.freecodecamp.org/">freeCodeCamp</a>. I have a
      background in Systems Administration and I wish to move my career towards
      full stack web development. You can follow my progress
      <a href="https://github.com/Seventy9/100-days-of-code/blob/master/log.md"
        >here</a
      >
      as I update my #100DaysOfCode challenge.
    </p>
  </div>
</template>

<style lang="scss">
#about {
  align-items: center;
  background-color: var(--main-grey);
  color: var(--main-white);
  display: flex;
  flex-direction: column;
  padding: 10rem 2rem;
  width: 100%;
}

#about-image {
  border-radius: 50%;
  height: 200px;
  margin-bottom: 5rem;
  width: 200px;
}

#about-title {
  margin-bottom: 5rem;
}

#about-description {
  max-width: 80rem;
}
</style>
