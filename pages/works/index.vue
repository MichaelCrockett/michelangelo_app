<template lang="html">
  <section class='works'>
    <Work
      v-for="work in works"
      :key="work.id"
      :thumbnail="work.thumbnail"
      :title="work.title"
      :id="work.id"
      :previewText="work.previewText"



      />
  </section>
</template>

<script>
import Work from '@/components/Work';

export default {
  components: {
    Work
  },
  asyncData() {
    return new Promise((resolve, reject) => {
      setTimeout(() => {
        resolve({
          works: [
            {
              id: "1",
              title: "Pieta",
              previewText: "The Pietà is a work of Renaissance sculpture by Michelangelo Buonarroti, housed in St. Peter's Basilica, Vatican City.",
              thumbnail: "https://upload.wikimedia.org/wikipedia/commons/6/6c/Michelangelo%27s_Pieta_5450_cut_out_black.jpg"
            },
            {
              id: "2",
              title: "Sistine Chapel",
              previewText: "The Sistine Chapel ceiling, painted by Michelangelo between 1508 and 1512, is a cornerstone work of High Renaissance art.",
              thumbnail: "https://www.thecollector.com/wp-content/uploads/2020/05/sistine_chapel_painted_frescoes_by_michelangelo_in_vatican_featured.jpg"
            },
            {
              id: "3",
              title: "David",
              previewText: "David is a masterpiece of Renaissance sculpture, created in marble between 1501 and 1504 by the Italian artist Michelangelo.",
              thumbnail: "https://s3-prod.modernhealthcare.com/s3fs-public/David_WEB_edit.jpg"
            },
            {
              id: "4",
              title: "Moses",
              previewText: "Moses is a sculpture by the Italian High Renaissance artist Michelangelo, housed in the church of San Pietro in Vincoli.",
              thumbnail: "https://anamericaninrome.com/wp/wp-content/uploads/2018/09/Michelangelo-Moses-7-1024x683.jpg"
            },
          ]
        })
      }, 1500)
    })
  }
};
</script>

<style scoped>

.works {
  display: flex;
  flex-flow: row wrap;
  justify-content: center;
  align-items: center;
}


</style>
