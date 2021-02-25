<template>
  <div id="contact">
    <h3 id="contact-title">
      Please feel free to contact me on:
    </h3>
    <div id="contact-list">
      <a class="contact-list-link" href="https://twitter.com/seventy9dev">
        <i class="fab fa-twitter-square contact-list-image"></i>Twitter
      </a>
      <a
        class="contact-list-link"
        href="https://www.linkedin.com/in/allen-parish-643ba530/"
      >
        <i class="fab fa-linkedin contact-list-image"></i>LinkedIn
      </a>
      <a class="contact-list-link" href="https://github.com/Seventy9">
        <i class="fab fa-github-square contact-list-image"></i>GitHub
      </a>
      <a class="contact-list-link" href="https://www.facebook.com/allenparish">
        <i class="fab fa-facebook-square contact-list-image"></i>Facebook
      </a>
    </div>
    <p id="contact-email">
      Or send me an email using the below form
    </p>
    <form
      id="contact-form"
      action="mailto:hello@seventy9.dev"
      method="POST"
      enctype="text/plain"
    >
      <label for="name">Name:</label>
      <input
        type="text"
        name="name"
        id="name"
        placeholder="Enter your name here..."
      />
      <label for="email">Email:</label>
      <input
        type="email"
        name="email"
        id="email"
        placeholder="Enter your email here..."
      />
      <label for="message">Message:</label>
      <textarea
        name="message"
        id="message"
        placeholder="Enter your message here..."
      ></textarea>
      <button id="contact-form-button" type="submit">Send Message</button>
    </form>
  </div>
</template>

<style lang="scss">
#contact {
  align-items: center;
  display: flex;
  flex-direction: column;
  justify-content: center;
  padding: 10rem 2rem;
}

#contact-title {
  margin-bottom: 5rem;
  max-width: 80rem;
}

#contact-list {
  display: flex;
  justify-content: space-between;
  margin-bottom: 5rem;
  max-width: 80rem;
  width: 100%;
}

.contact-list-link {
  color: var(--text-dark);
  font-size: 2rem;
}

.contact-list-link:hover {
  color: var(--highlight-dark);
}

.contact-list-image {
  margin: 0 1rem;
}

#contact-email {
  margin-bottom: 5rem;
}

#contact-form {
  display: flex;
  flex-direction: column;
  max-width: 80rem;
  width: 100%;
}

#name,
#email {
  background-color: var(--background-light);
  border: 0.1rem solid var(--text-dark);
  border-radius: 1rem;
  font-family: "Asap", sans-serif;
  font-size: 1.6rem;
  font-weight: 400;
  margin: 1.6rem 0;
  padding: 1rem;
  width: 100%;
}

#message {
  background-color: var(--background-light);
  border: 0.1rem solid var(--text-dark);
  border-radius: 1rem;
  font-family: "Asap", sans-serif;
  font-size: 1.6rem;
  font-weight: 400;
  height: 10rem;
  margin: 1.6rem 0;
  padding: 1rem;
  width: 100%;
}

#name:focus,
#email:focus,
#message:focus {
  outline-width: 0;
}

#contact-form-button {
  background-color: var(--background-dark);
  border: none;
  border-radius: 1rem;
  color: var(--text-light);
  font-family: "Asap", sans-serif;
  font-size: 2.4rem;
  font-weight: 400;
  padding: 1rem;
  text-transform: uppercase;
  transition: 0.3s;
}

#contact-form-button:hover {
  background-color: var(--highlight-dark);
  cursor: pointer;
}

@media (max-width: 768px) {
  #contact-list {
    align-items: flex-start;
    flex-direction: column;
    width: 200px;
  }
  .contact-list-link:not(:last-child) {
    margin-bottom: 1.6rem;
  }
}
</style>
