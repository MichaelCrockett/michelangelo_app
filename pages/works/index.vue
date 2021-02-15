<template lang="html">
  <section class='works'>
    <article class="work">
      <div class="thumbnail" style="background-image: url('https://upload.wikimedia.org/wikipedia/commons/6/6c/Michelangelo%27s_Pieta_5450_cut_out_black.jpg')"></div>
      <h1>Pieta</h1>
      <p>The Pietà is a work of Renaissance sculpture by Michelangelo Buonarroti, housed in St. Peter's Basilica, Vatican City.</p>
    </article>
    <article class="work">
      <div class="thumbnail" style="background-image: url('https://www.thecollector.com/wp-content/uploads/2020/05/sistine_chapel_painted_frescoes_by_michelangelo_in_vatican_featured.jpg')"></div>
      <h1>Sistine Chapel Ceiling</h1>
      <p>The Sistine Chapel ceiling (Italian: Volta della Cappella Sistina), painted by Michelangelo between 1508 and 1512, is a cornerstone work of High Renaissance art.</p>
    </article>
    <article class="work">
      <div class="thumbnail" style="background-image: url('https://s3-prod.modernhealthcare.com/s3fs-public/David_WEB_edit.jpg')"></div>
      <h1>David</h1>
      <p>David is a masterpiece of Renaissance sculpture, created in marble between 1501 and 1504 by the Italian artist Michelangelo. David is a 5.17-metre (17.0 ft) marble statue of the Biblical figure David.</p>
    </article>
    <article class="work">
      <div class="thumbnail" style="background-image: url('https://anamericaninrome.com/wp/wp-content/uploads/2018/09/Michelangelo-Moses-7-1024x683.jpg')"></div>
      <h1>Moses</h1>
      <p>Moses is a sculpture by the Italian High Renaissance artist Michelangelo Buonarroti, housed in the church of San Pietro in Vincoli in Rome.</p>
    </article>
  </section>
</template>

<script>
export default {
}
</script>

<style lang="css" scoped>
.works {
  display: flex;
  flex-flow: row wrap;
  justify-content: center;
  align-items: center;
}

.work {
  box-sizing: border-box;
  width: 280px;
  padding: 8px;
  border: 1px solid #ccc;
  box-shadow: 0 2px 2px #aaa;
  margin: 10px;
}

.thumbnail {
  background-position: center;
  background-size: cover;
  width: 100%;
  height: 200px;
}

</style>
