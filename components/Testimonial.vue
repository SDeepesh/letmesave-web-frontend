<template>
    <div class="testimonial-sec">
      <h4>With love to Letme-save.com</h4>
      <v-container>
        <v-sheet>
        <v-slide-group
          v-model="model"
          class="custom-test"
          center-active
          show-arrows
        >
          <v-slide-item>
            <v-card
              class="ma-4"
              height="200"
              width="500"
            >
              <v-row
                class="fill-height"
                align="center"
                justify="center"
              >
              <div>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua</div>
                <v-scale-transition>
                  <v-icon
                    v-if="active"
                    color="white"
                    size="48"
                    v-text="'mdi-close-circle-outline'"
                  ></v-icon>
                </v-scale-transition>
              </v-row>
            </v-card>
          </v-slide-item>
          <v-slide-item>
            <v-card
              class="ma-4"
              height="200"
              width="500"
            >
              <v-row
                class="fill-height"
                align="center"
                justify="center"
              >
              <div>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua</div>
                <v-scale-transition>
                  <v-icon
                    v-if="active"
                    color="white"
                    size="48"
                    v-text="'mdi-close-circle-outline'"
                  ></v-icon>
                </v-scale-transition>
              </v-row>
            </v-card>
          </v-slide-item>
          <v-slide-item>
            <v-card
              class="ma-4"
              height="200"
              width="500"
            >
              <v-row
                class="fill-height"
                align="center"
                justify="center"
              >
              <div class="testimonial-content">
                <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua</p>
              </div>
                <v-scale-transition>
                  <v-icon
                    v-if="active"
                    color="white"
                    size="48"
                    v-text="'mdi-close-circle-outline'"
                  ></v-icon>
                </v-scale-transition>
              </v-row>
            </v-card>
          </v-slide-item>
        </v-slide-group>
      </v-sheet>
      </v-container>
    </div>

</template>

<style scoped>
.testimonial-sec {
    background-image: url("../assets/pic-12.jpg");
    background-position: center;
    background-size: cover;
    background-repeat: no-repeat;
    text-align: center;
    margin-top: 3em;
    padding:3em 0;
}
.testimonial-sec h4{
  font-size: 48px;
  font-weight: 300;
  color: #fff;
}
</style>

