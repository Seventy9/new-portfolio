<template>
  <nav id="navigation">
    <a href="#header" class="logo"> <i class="fas fa-code"></i> Seventy9 </a>
    <input class="menu-btn" type="checkbox" id="menu-btn" />
    <label class="menu-icon" for="menu-btn">
      <span class="navicon"></span>
    </label>
    <ul class="menu">
      <li><a href="#about">About</a></li>
      <li><a href="#skills">Skills</a></li>
      <li><a href="#projects">Projects</a></li>
      <li><a href="#contact">Contact</a></li>
    </ul>
  </nav>
</template>

<style lang="scss">
#navigation {
  background-color: var(--background-dark);
  border-bottom: 2px solid var(--highlight-light);
  left: 0;
  line-height: 1rem;
  position: fixed;
  top: 0;
  width: 100%;
  z-index: 10;
}

#navigation a {
  color: var(--highlight-light);
}

#navigation ul {
  list-style: none;
  overflow: hidden;
}

#navigation li a {
  display: block;
  padding: 2rem;
  text-decoration: none;
}

#navigation li a:hover,
#navigation .menu-btn:hover {
  background-color: var(--background-light);
  color: var(--main-black);
  transition: 0.3s;
}

#navigation .logo {
  display: block;
  float: left;
  font-size: 2rem;
  padding: 1.5rem 2rem;
  text-decoration: none;
}

#navigation .menu {
  clear: both;
  max-height: 0;
  transition: max-height 0.2s ease-out;
}

#navigation .menu-icon {
  cursor: pointer;
  float: right;
  padding: 28px 20px;
  position: relative;
  user-select: none;
}

#navigation .menu-icon .navicon {
  background: var(--main-white);
  display: block;
  height: 2px;
  position: relative;
  transition: background 0.2s ease-out;
  width: 18px;
}

#navigation .menu-icon .navicon:before,
#navigation .menu-icon .navicon:after {
  background: var(--background-light);
  content: "";
  display: block;
  height: 100%;
  position: absolute;
  transition: all 0.2s ease-out;
  width: 100%;
}

#navigation .menu-icon .navicon:before {
  top: 5px;
}

#navigation .menu-icon .navicon:after {
  top: -5px;
}

#navigation .menu-btn {
  display: none;
}

#navigation .menu-btn:checked ~ .menu {
  max-height: 240px;
}

#navigation .menu-btn:checked ~ .menu-icon .navicon {
  background: transparent;
}

#navigation .menu-btn:checked ~ .menu-icon .navicon:before {
  transform: rotate(-45deg);
}

#navigation .menu-btn:checked ~ .menu-icon .navicon:after {
  transform: rotate(45deg);
}

#navigation .menu-btn:checked ~ .menu-icon:not(.steps) .navicon:before,
#navigation .menu-btn:checked ~ .menu-icon:not(.steps) .navicon:after {
  top: 0;
}

@media (min-width: 768px) {
  #navigation li {
    float: left;
  }
  #navigation li a {
    padding: 20px 30px;
  }
  #navigation .menu {
    clear: none;
    float: right;
    max-height: none;
  }
  #navigation .menu-icon {
    display: none;
  }
}
</style>
