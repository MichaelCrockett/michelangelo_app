<template>
  <div class="container">
      <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/0/02/Michelangelo_Daniele_da_Volterra_%28dettaglio%29.jpg/220px-Michelangelo_Daniele_da_Volterra_%28dettaglio%29.jpg" alt="Michelangelo" class="mich-pic">
      <h1 class="title">
        The works of Michelangelo
      </h1>
      <br><br>
      <quote>"If you knew how much work it took, you wouldn't call it genius"</quote>
    </div>
  </div>
</template>

<script>
export default {

}
</script>

<style>
.container {
  margin: 0 auto;
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
}
.mich-pic {
  width: 30%;
}

.title {
  font-family:
    'Quicksand',
    'Source Sans Pro',
    -apple-system,
    BlinkMacSystemFont,
    'Segoe UI',
    Roboto,
    'Helvetica Neue',
    Arial,
    sans-serif;
  display: block;
  font-weight: 300;
  font-size: 100px;
  color: #35495e;
  letter-spacing: 1px;
}

.subtitle {
  font-weight: 300;
  font-size: 42px;
  color: #526488;
  word-spacing: 5px;
  padding-bottom: 15px;
}

.links {
  padding-top: 15px;
}
</style>
