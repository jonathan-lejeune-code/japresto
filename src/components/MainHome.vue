<template>
  <v-app>
    <section>
      <v-layout column wrap class="my-5" align-center>
        <v-flex xs12 sm4 class="my-3">
          <div class="text-xs-center">
            <h2 class="headline">
              La cuisine typique japonaise dans votre cuisine
            </h2>
            <span class="subheading"> キッチンでの典型的な日本料理 </span>
          </div>
        </v-flex>
        <v-flex>
          <v-container grid-list-xl>
            <v-layout row wrap align-center>
              <v-flex xs12 md4>
                <v-card class="elevation-0 transparent" height="600">
                  <v-card-text class="text-xs-center"> </v-card-text>
                  <v-card-title primary-title class="layout justify-center">
                    <v-icon x-large class="red--text text--darken-2"
                      >mdi-home</v-icon
                    >
                    <div class="headline">Produit frais</div>
                  </v-card-title>
                  <v-img
                    src="https://media.istockphoto.com/photos/salmon-sashimi-picture-id185319629?k=20&m=185319629&s=612x612&w=0&h=Pt5iG5f4I9UYfRf2DlWml5v4zj6LA5jsrQjuKawGj-o="
                    alt="image sushi"
                    height="300"
                  />
                  <v-card-text>
                    Cras facilisis mi vitae nunc lobortis pharetra. Nulla
                    volutpat tincidunt ornare. Pellentesque habitant morbi
                    tristique senectus et netus et malesuada fames ac turpis
                    egestas. Nullam in aliquet odio.
                  </v-card-text>
                </v-card>
              </v-flex>
              <v-flex xs12 md4>
                <v-card class="elevation-0 transparent" height="600">
                  <v-card-text class="text-xs-center"> </v-card-text>
                  <v-card-title primary-title class="layout justify-center">
                    <v-icon x-large class="red--text text--darken-2"
                      >mdi-knife</v-icon
                    >
                    <div class="headline">Préparation sur place</div>
                  </v-card-title>
                  <v-img
                    src="https://thumbs.dreamstime.com/b/male-person-cooking-sushi-japanese-food-wooden-table-preparation-process-traditional-asian-cuisine-seafood-delicious-108224976.jpg"
                    alt="image sushi"
                    height="300"
                  />
                  <v-card-text>
                    Pellentesque habitant morbi tristique senectus et netus et
                    malesuada fames ac turpis egestas. Nullam in aliquet odio.
                    Aliquam eu est vitae tellus bibendum tincidunt. Suspendisse
                    potenti.
                  </v-card-text>
                </v-card>
              </v-flex>
              <v-flex xs12 md4>
                <v-card class="elevation-0 transparent" height="600">
                  <v-card-text class="text-xs-center"> </v-card-text>
                  <v-card-title primary-title class="layout justify-center">
                    <v-icon x-large class="red--text text--darken-2"
                      >mdi-fish</v-icon
                    >
                    <div class="headline text-xs-center">
                      Grand choix de plats
                    </div>
                  </v-card-title>
                  <v-img
                    src="https://www.otodoke.fr/wp-content/uploads/2018/05/japan-feat.jpg"
                    alt="Vuetify.js"
                    height="300"
                  />
                  <v-card-text>
                    Cras facilisis mi vitae nunc lobortis pharetra. Nulla
                    volutpat tincidunt ornare. Pellentesque habitant morbi
                    tristique senectus et netus et malesuada fames ac turpis
                    egestas. Nullam in aliquet odio. Aliquam eu est vitae tellus
                    bibendum tincidunt. Suspendisse potenti.
                  </v-card-text>
                </v-card>
              </v-flex>
            </v-layout>
          </v-container>
        </v-flex>
      </v-layout>
    </section>
    <section>
      <v-parallax
        src="https://wallpaperaccess.com/full/1321841.gif"
        height="380"
      >
        <v-layout column align-center justify-center>
          <div class="headline white--text mb-3 text-xs-center">
            Aller voir notre page des menu pour voir nos plats
          </div>
          <em>あなたはあなたの幸せを見つけるでしょう</em>
          <v-btn class="red darken-2 mt-5" dark large href="/menu">
            Menu
          </v-btn>
        </v-layout>
      </v-parallax>
    </section>
  </v-app>
</template>

<script>
export default {};
</script>

<style></style>
