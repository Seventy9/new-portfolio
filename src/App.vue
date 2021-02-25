<template>
  <Navigation />
  <Header />
  <About />
  <Skills />
  <Projects />
  <Contact />
  <Footer />
</template>

<script>
import Navigation from "./components/Navigation";
import Header from "./components/Header";
import About from "./components/About";
import Skills from "./components/Skills";
import Projects from "./components/Projects";
import Contact from "./components/Contact";
import Footer from "./components/Footer";

export default {
  name: "App",
  components: {
    Navigation,
    Header,
    About,
    Skills,
    Projects,
    Contact,
    Footer
  }
};
</script>

<style lang="scss">
:root {
  --main-black: #222831;
  --main-grey: #393e46;
  --main-white: #e8f1ff;
  --main-yellow: #ffa500;
  --background-light: #e8f1ff;
  --background-dark: #393e46;
  --text-light: #e8f1ff;
  --text-dark: #393e46;
  --highlight-light: #ffa500;
  --highlight-dark: #004194;
}

* {
  margin: 0;
  padding: 0;
}

*,
*::before,
*::after {
  box-sizing: inherit;
}

html {
  box-sizing: border-box;
  font-size: 62.5%;
  scroll-behavior: smooth;
}

a {
  color: var(--main-yellow);
  text-decoration: none;
}

a:hover {
  text-decoration: none;
}

body {
  background-color: var(--background-light);
  color: var(--text-dark);
  font-family: "Asap", sans-serif;
  font-size: 1.6rem;
  font-weight: 400;
  line-height: 1.6rem;
}

h1,
h2,
h3,
h4,
h5,
h6 {
  font-weight: 700;
  text-align: center;
}

h1 {
  font-size: 6.4rem;
  line-height: 6.4rem;
}

h2 {
  font-size: 5.2rem;
  line-height: 5.2rem;
}

h3 {
  font-size: 4rem;
  line-height: 4rem;
}

h4 {
  font-size: 3.2rem;
  line-height: 3.2rem;
}

h5 {
  font-size: 2.4rem;
  line-height: 2.4rem;
}

h6 {
  font-size: 2rem;
  line-height: 2rem;
}

img {
  display: block;
  width: 100%;
}

ul {
  list-style: none;
}
</style>
