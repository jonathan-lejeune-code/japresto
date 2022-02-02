<template>
  <section>
    <v-container grid-list-xl>
      <v-layout row wrap justify-center class="my-5">
        <v-flex xs12 sm4>
          <v-card class="elevation-0 transparent">
            <v-card-title primary-title class="layout justify-center">
              <div class="headline">Informations</div>
            </v-card-title>
            <v-card-text>
              Cras facilisis mi vitae nunc lobortis pharetra. Nulla volutpat
              tincidunt ornare. Pellentesque habitant morbi tristique senectus
              et netus et malesuada fames ac turpis egestas. Nullam in aliquet
              odio. Aliquam eu est vitae tellus bibendum tincidunt. Suspendisse
              potenti.
            </v-card-text>
          </v-card>
        </v-flex>
        <v-flex xs12 sm4 offset-sm1>
          <v-card class="elevation-0 transparent">
            <v-card-title primary-title class="layout justify-center">
              <div class="headline">Contact</div>
            </v-card-title>
            <v-card-text>
              Cras facilisis mi vitae nunc lobortis pharetra. Nulla volutpat
              tincidunt ornare.
            </v-card-text>
            <v-list class="transparent">
              <v-list-tile>
                <v-list-tile-action>
                  <v-icon class="red--text text--darken-2 ml-10 mr-2"
                    >mdi-phone</v-icon
                  >
                </v-list-tile-action>
                <v-list-tile-content>
                  <v-list-tile-title>777-867-5309</v-list-tile-title>
                </v-list-tile-content>
              </v-list-tile>
              <v-list-tile>
                <v-list-tile-action>
                  <v-icon class="red--text text--darken-2 ml-10 mr-2"
                    >mdi-city</v-icon
                  >
                </v-list-tile-action>
                <v-list-tile-content>
                  <v-list-tile-title>Aaaaaaa, AAA</v-list-tile-title>
                </v-list-tile-content>
              </v-list-tile>
              <v-list-tile>
                <v-list-tile-action>
                  <v-icon class="red--text text--darken-2 ml-10 mr-2"
                    >mdi-email</v-icon
                  >
                </v-list-tile-action>
                <v-list-tile-content>
                  <v-list-tile-title>john@mail.com</v-list-tile-title>
                </v-list-tile-content>
              </v-list-tile>
            </v-list>
          </v-card>
        </v-flex>
        <iframe
          src="https://www.google.com/maps/embed?pb=!1m14!1m12!1m3!1d10417117.66444122!2d13.002410974316424!3d50.3993345390241!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!5e0!3m2!1sfr!2sfr!4v1643467680228!5m2!1sfr!2sfr"
          :center="center"
          :zoom="12"
          style="width: 100%; height: 400px"
          allowfullscreen=""
          loading="lazy"
        ></iframe>
      </v-layout>
    </v-container>
  </section>
</template>

<script>
export default {};
</script>

<style></style>
