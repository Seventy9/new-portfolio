<template>
  <div id="footer">
    <p id="footer-text">© {{ getYear() }} Allen Parish</p>
  </div>
</template>

<script>
export default {
  methods: {
    getYear() {
      return new Date().getFullYear();
    }
  }
};
</script>

<style lang="scss">
#footer {
  background-color: var(--background-dark);
  border-top: 0.2rem solid var(--highlight-light);
  color: var(--text-light);
  display: flex;
  justify-content: center;
  padding: 2rem 0;
  width: 100%;
}

#footer-text {
  text-align: right;
  margin-right: 1rem;
  width: 80rem;
}
</style>
