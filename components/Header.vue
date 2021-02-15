<template lang="html">
  <header>
    <nav>
      <ul>
        <li><nuxt-link to="/">Start page</nuxt-link></li>
        <li><nuxt-link to="/works">Works of art</nuxt-link></li>
        <li><nuxt-link to="/about">About</nuxt-link></li>
      </ul>
    </nav>
  </header>
</template>


<style scoped>

header {
  width: 100%;
  height: 60px;
  display: flex;
  justify-content: center;
  align-items: center;
  background-color: wheat;
}

ul {
  list-style: none;
  margin: 0;
  padding: 0;
  display: flex;
  justify-content: center;
  align-items: center;
}

li {
  margin: 0 10px;
}
a {
  text-decoration: none;
  color: black;
}

</style>
