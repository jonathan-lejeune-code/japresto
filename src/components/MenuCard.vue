<template>
  <v-row>
    <v-col>
      <v-card-title class="title2">Menu</v-card-title>
      <v-col cols="12">
        <v-card
          style="
            display: flex;
            flex-wrap: wrap;
            flex-direction: row;
            justify-content: space-between;
          "
          class="cards"
        >
          <v-card-item v-for="(menu, i) in menus" :key="i" small>
            <div>
              <v-card
                color="red darken-2"
                class="white--text"
                style="margin: 20px; width: 300px; height: auto"
              >
                <v-img
                  class="img hidden-xs-only headshot-1"
                  height="200"
                  :src="menu.src"
                ></v-img>

                <v-card-title>
                  <div>
                    <div
                      :class="`headline font-italic`"
                      style="
                        display: flex;
                        flex-wrap: wrap;
                        flex-direction: row;
                        justify-content: flex-start;
                      "
                    >
                      {{ menu.title }}
                      <div>
                        <v-spacer></v-spacer>
                        <v-btn
                          icon
                          @click="menu.show = !menu.show"
                          color="white"
                        >
                          <v-icon>{{
                            menu.show ? "mdi-chevron-up" : "mdi-chevron-down"
                          }}</v-icon>
                        </v-btn>
                        <v-expand-transition>
                          <div v-show="menu.show">
                            <v-divider></v-divider>

                            <v-card-text
                              style="min-height: 250px"
                              class="white--text"
                            >
                              {{ menu.comment }}
                            </v-card-text>
                            <v-card-text
                              style="font-size: 30px"
                              class="font-weight-black white--text font-italic shotprice"
                            >
                              {{ menu.prix }}€
                            </v-card-text>
                          </div>
                        </v-expand-transition>
                      </div>
                    </div>
                  </div>
                </v-card-title>
              </v-card>
            </div>
          </v-card-item>
        </v-card>
      </v-col>
    </v-col>
  </v-row>
</template>

<script>
export default {
  data: () => ({
    menus: [
      {
        title: " Nouille aux oeuf ",

        src: "https://sp-ao.shortpixel.ai/client/to_webp,q_glossy,ret_img,w_1024,h_682/https://nihonkara.fr/wp-content/uploads/2017/11/Ramen-1024x682.jpg",
        comment:
          "Lorem ipsum dolor sit amet. Aut nemo distinctio in omnis vitae id animi neque ea iusto corporis et voluptatibus dolor qui nisi cumque. Et fugiat enim id dolorum magni est nobis quasi. Et odit quia non animi cupiditate qui tenetur consequatur. ",
        prix: "5",
        show: false,
      },
      {
        title: " Poulet caramel  ",

        src: `https://foodscene.deliveroo.fr/assets/images/blogs/foodscene.deliveroo.fr/fr/inspiration-culinaire/1nys62vCPp5vRm3K7XyRnswd1sLWVvrtgbYpj4mXMICs/h_6._japanese_curries.jpg?v=1.01`,
        comment:
          "Lorem ipsum dolor sit amet. Aut nemo distinctio in omnis vitae id animi neque ea iusto corporis et voluptatibus dolor qui nisi cumque. Et fugiat enim id dolorum magni est nobis quasi. Et odit quia non animi cupiditate qui tenetur consequatur. ",
        prix: "7",
        show: false,
      },
      {
        title: " Riz aux oeuf ",

        src: "https://www.qooq.com/sites/default/files/styles/main_photo/public/externals/2455.jpg?itok=c5MfAA-2",
        comment:
          "Lorem ipsum dolor sit amet. Aut nemo distinctio in omnis vitae id animi neque ea iusto corporis et voluptatibus dolor qui nisi cumque. Et fugiat enim id dolorum magni est nobis quasi. Et odit quia non animi cupiditate qui tenetur consequatur. ",
        prix: "3",
        show: false,
      },
      {
        title: " Brochette de poulet  ",

        src: "https://allomamantoutvabien.com/wp-content/uploads/2017/02/takoyaki-7-1.jpg",
        comment:
          "Lorem ipsum dolor sit amet. Aut nemo distinctio in omnis vitae id animi neque ea iusto corporis et voluptatibus dolor qui nisi cumque. Et fugiat enim id dolorum magni est nobis quasi. Et odit quia non animi cupiditate qui tenetur consequatur. ",
        prix: "8",
        show: false,
      },
      {
        title: " Brochette caramelisé ",

        src: "https://www.terres-japonaises.com/app/media/26/files/2016/06/yakitori-japon.jpg",
        comment:
          "Lorem ipsum dolor sit amet. Aut nemo distinctio in omnis vitae id animi neque ea iusto corporis et voluptatibus dolor qui nisi cumque. Et fugiat enim id dolorum magni est nobis quasi. Et odit quia non animi cupiditate qui tenetur consequatur. ",
        prix: "7",
        show: false,
      },
      {
        title: " Sushi ",

        src: "https://www.restaurant-inagiku.fr/wp-content/uploads/2020/12/Assiette-de-sushis-1170x550.jpg",
        comment:
          "Lorem ipsum dolor sit amet. Aut nemo distinctio in omnis vitae id animi neque ea iusto corporis et voluptatibus dolor qui nisi cumque. Et fugiat enim id dolorum magni est nobis quasi. Et odit quia non animi cupiditate qui tenetur consequatur. ",
        prix: "9",
        show: false,
      },
      {
        title: " Nouille avec légumes ",

        src: "https://www.alvo.be/sites/default/files/styles/large/public/pictures/recipes/japanse-groenteschotel-noodles-kl.jpg?itok=YPY6mA-A",
        comment:
          "Lorem ipsum dolor sit amet. Aut nemo distinctio in omnis vitae id animi neque ea iusto corporis et voluptatibus dolor qui nisi cumque. Et fugiat enim id dolorum magni est nobis quasi. Et odit quia non animi cupiditate qui tenetur consequatur. ",
        prix: "7",
        show: false,
      },
      {
        title: " Gyoza ",

        src: "https://www.maspatule.com/blog/wp-content/uploads/2020/01/mise-en-avant-gyoza-1440x1128.jpg",
        comment:
          "Lorem ipsum dolor sit amet. Aut nemo distinctio in omnis vitae id animi neque ea iusto corporis et voluptatibus dolor qui nisi cumque. Et fugiat enim id dolorum magni est nobis quasi. Et odit quia non animi cupiditate qui tenetur consequatur. ",
        prix: "7",
        show: false,
      },
      {
        title: " Nems ",

        src: "https://files.meilleurduchef.com/mdc/photo/recette/pate-chinois/pate-chinois-800.jpg",
        comment:
          "Lorem ipsum dolor sit amet. Aut nemo distinctio in omnis vitae id animi neque ea iusto corporis et voluptatibus dolor qui nisi cumque. Et fugiat enim id dolorum magni est nobis quasi. Et odit quia non animi cupiditate qui tenetur consequatur. ",
        prix: "7",
        show: false,
      },
      {
        title: " Ramen ",

        src: "https://res.cloudinary.com/serdy-m-dia-inc/image/upload/f_auto/fl_lossy/q_auto:eco/x_0,y_104,w_3840,h_2160,c_crop/w_1200,h_630,c_fill/v1545089694/foodlavie/prod/recettes/soupe-ramen-au-curry-rouge-42123da9",
        comment:
          "Lorem ipsum dolor sit amet. Aut nemo distinctio in omnis vitae id animi neque ea iusto corporis et voluptatibus dolor qui nisi cumque. Et fugiat enim id dolorum magni est nobis quasi. Et odit quia non animi cupiditate qui tenetur consequatur. ",
        prix: "9",
        show: false,
      },
      {
        title: " Miso facon Mérope ",

        src: require("../assets/nouillemérope.jpeg"),
        comment:
          "Lorem ipsum dolor sit amet. Aut nemo distinctio in omnis vitae id animi neque ea iusto corporis et voluptatibus dolor qui nisi cumque. Et fugiat enim id dolorum magni est nobis quasi. Et odit quia non animi cupiditate qui tenetur consequatur. ",
        prix: "10",
        show: false,
      },
      {
        title: " Soupe facon Lucie ",

        src: require("../assets/nouille2.jpeg"),
        comment:
          "Lorem ipsum dolor sit amet. Aut nemo distinctio in omnis vitae id animi neque ea iusto corporis et voluptatibus dolor qui nisi cumque. Et fugiat enim id dolorum magni est nobis quasi. Et odit quia non animi cupiditate qui tenetur consequatur. ",
        prix: "10",
        show: false,
      },
    ],
  }),
};
</script>

<style>
.title2 {
  width: 300px;
  font-size: 40px;
  color: #d32f2f;
  margin: 30px auto 20px auto;
  border: #d32f2f solid 4px;
  flex-direction: column;
  font-family: "Dancing Script", cursive;
}

.headshot-1 {
  border-radius: 10% 60%;
  border: black solid 5px;
}

.shotprice {
  background-color: black;
  width: 80px;
  box-shadow: 6px 3px 9px white;

  border-radius: 40% 10%;
}

.cards {
  margin-left: auto;
  margin-right: auto;
}
</style>
