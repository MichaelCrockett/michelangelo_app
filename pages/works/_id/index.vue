<template lang="html">
  <section class="single-work">
    <h1>{{ work.title }}</h1>
    <div class="">
      <img class="work-image":src="work.thumbnail" :alt="work.title">
    </div>
    <br>
    <p>{{ work.descriptionText }}</p>
  </section>
</template>

<script>
  export default {
    asyncData(context) {
      return new Promise((resolve, reject) => {
        setTimeout(() => {
          resolve({
            work: [
              {
                id: "1",
                title: "Pieta",
                previewText: "The Pietà is a work of Renaissance sculpture by Michelangelo Buonarroti, housed in St. Peter's Basilica, Vatican City.",
                descriptionText: "The Pietà (Italian: [pjeˈta]; English: 'The Piety'; 1498–1499) is a work of Renaissance sculpture by Michelangelo Buonarroti, housed in St. Peter's Basilica, Vatican City.It is the first of a number of works of the same theme by the artist. The statue was commissioned for the French Cardinal Jean de Bilhères, who was a representative in Rome. The sculpture, in Carrara marble, was made for the cardinal's funeral monument, but was moved to its current location, the first chapel on the north side of the entrance of the basilica, in the 18th century. It is the only piece Michelangelo ever signed. It is also the only known sculpture created by a prominent name from the Renaissance era that was installed in St. Peter's Basilica that was accepted by the Chapter of St. Peter. This famous work of art depicts the body of Jesus on the lap of his mother Mary after the Crucifixion. The theme is of Northern origin. Michelangelo's interpretation of the Pietà is unprecedented in Italian sculpture. It is an important work as it balances the Renaissance ideals of classical beauty with naturalism. In 2019, a small terracotta figure identified as a model for the final sculpture was displayed in Paris.",
                thumbnail: "https://upload.wikimedia.org/wikipedia/commons/6/6c/Michelangelo%27s_Pieta_5450_cut_out_black.jpg"
              },
              {
                id: "2",
                title: "Sistine Chapel",
                previewText: "The Sistine Chapel ceiling, painted by Michelangelo between 1508 and 1512, is a cornerstone work of High Renaissance art.",
                descriptionText: "The Sistine Chapel ceiling (Italian: Volta della Cappella Sistina), painted by Michelangelo between 1508 and 1512, is a cornerstone work of High Renaissance art. The ceiling is that of the Sistine Chapel, the large papal chapel built within the Vatican between 1477 and 1480 by Pope Sixtus IV, for whom the chapel is named. It was painted at the commission of Pope Julius II. The chapel is the location for papal conclaves and many other important services.  The ceiling's various painted elements form part of a larger scheme of decoration within the Chapel, which includes the large fresco The Last Judgement on the sanctuary wall, also by Michelangelo, wall paintings by several leading painters of the late 15th century including Sandro Botticelli, Domenico Ghirlandaio and Pietro Perugino, and a set of large tapestries by Raphael, the whole illustrating much of the doctrine of the Catholic Church.  Central to the ceiling decoration are nine scenes from the Book of Genesis, of which The Creation of Adam is the best known, having an iconic standing equalled only by Leonardo da Vinci's Mona Lisa, the hands of God and Adam being reproduced in countless imitations. The complex design includes several sets of individual figures, both clothed and nude, which allowed Michelangelo to fully demonstrate his skill in creating a huge variety of poses for the human figure and which have provided an enormously influential pattern book of models for other artists ever since.",
                thumbnail: "https://www.thecollector.com/wp-content/uploads/2020/05/sistine_chapel_painted_frescoes_by_michelangelo_in_vatican_featured.jpg"
              },
              {
                id: "3",
                title: "David",
                previewText: "David is a masterpiece of Renaissance sculpture, created in marble between 1501 and 1504 by the Italian artist Michelangelo.",
                descriptionText: "David is a masterpiece of Renaissance sculpture, created in marble between 1501 and 1504 by the Italian artist Michelangelo. David is a 5.17-metre (17.0 ft)[a] marble statue of the Biblical figure David, a favoured subject in the art of Florence.  David was originally commissioned as one of a series of statues of prophets to be positioned along the roofline of the east end of Florence Cathedral, but was instead placed in a public square, outside the Palazzo Vecchio, the seat of civic government in Florence, in the Piazza della Signoria, where it was unveiled on 8 September, 1504. The statue was moved to the Galleria dell'Accademia, Florence, in 1873, and later replaced at the original location by a replica.  Because of the nature of the figure it represented, the statue soon came to symbolize the defence of civil liberties embodied in the Republic of Florence, an independent city-state threatened on all sides by more powerful rival states and by the hegemony of the Medici family. The eyes of David, with a warning glare, were fixated towards Rome.",
                thumbnail: "https://s3-prod.modernhealthcare.com/s3fs-public/David_WEB_edit.jpg"
              },
              {
                id: "4",
                title: "Moses",
                previewText: "Moses is a sculpture by the Italian High Renaissance artist Michelangelo, housed in the church of San Pietro in Vincoli.",
                descriptionText: "Moses (Italian: Mosè [moˈzɛ]; c. 1513–1515) is a sculpture by the Italian High Renaissance artist Michelangelo Buonarroti, housed in the church of San Pietro in Vincoli in Rome.[2] Commissioned in 1505 by Pope Julius II for his tomb, it depicts the biblical figure Moses with horns on his head, based on a description in chapter 34 of Exodus in the Vulgate, the Latin translation of the Bible used at that time.",
                thumbnail: "https://anamericaninrome.com/wp/wp-content/uploads/2018/09/Michelangelo-Moses-7-1024x683.jpg"
              },
            ].find(el => el.id === context.params.id)
          })
        }, 1000)
      })
    }
  }
</script>

<style scoped>
  .single-work {
    display: flex;
    flex-flow: column;
    justify-content: center;
    align-items: center;
    text-align: center;
    padding: 30px;
  }

  .work-image {
    width: 400px;
  }
</style>
