<template lang="html">
  <section class='works'>
    <Work thumbnail="https://upload.wikimedia.org/wikipedia/commons/6/6c/Michelangelo%27s_Pieta_5450_cut_out_black.jpg"
    title="Pieta"
    previewText="The Pietà is a work of Renaissance sculpture by Michelangelo Buonarroti, housed in St. Peter's Basilica, Vatican City." />

    <Work thumbnail="https://www.thecollector.com/wp-content/uploads/2020/05/sistine_chapel_painted_frescoes_by_michelangelo_in_vatican_featured.jpg"
    title="Sistine Chapel"
    previewText="The Sistine Chapel ceiling, painted by Michelangelo between 1508 and 1512, is a cornerstone work of High Renaissance art." />

    <Work thumbnail="https://s3-prod.modernhealthcare.com/s3fs-public/David_WEB_edit.jpg"
    title="David"
    previewText="David is a masterpiece of Renaissance sculpture, created in marble between 1501 and 1504 by the Italian artist Michelangelo." />

    <Work thumbnail="https://anamericaninrome.com/wp/wp-content/uploads/2018/09/Michelangelo-Moses-7-1024x683.jpg"
    title="Moses"
    previewText="Moses is a sculpture by the Italian High Renaissance artist Michelangelo, housed in the church of San Pietro in Vincoli." />
  </section>
</template>

<script>
import Work from '@/components/Work'

export default {
  components: {
    Work
  }
}
</script>

<style scoped>

.works {
  display: flex;
  flex-flow: row wrap;
  justify-content: center;
  align-items: center;
}


</style>
