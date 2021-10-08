<template>
  <div class="block galleryBlock">
    <v-container>
      <h2 class="text-center">Gallery</h2>
      <v-row>
        <v-col
          v-for="item in items"
          :key="item.id"
          class="d-flex child-flex"
          cols="4"
        >
          <v-img
            :src="item.src"
            :lazy-src="item.src"
            aspect-ratio="1"
            class="grey lighten-2"
          >
            <template v-slot:placeholder>
              <v-row class="fill-height ma-0" align="center" justify="center">
                <v-progress-circular
                  indeterminate
                  color="grey lighten-5"
                ></v-progress-circular>
              </v-row>
            </template>
          </v-img>
        </v-col>
      </v-row>
    </v-container>
  </div>
</template>

<script>
export default {
  data() {
    return {
      items: [
        {
          src: require('../assets/images/img1.jpg'),
        },
        {
          src: require('../assets/images/img2.jpg'),
        },
        {
          src: require('../assets/images/img3.jpg'),
        },
        {
          src: require('../assets/images/img4.jpg'),
        },
        {
          src: require('../assets/images/img5.jpg'),
        },
        {
          src: require('../assets/images/img6.jpg'),
        },
        {
          src: require('../assets/images/img7.jpg'),
        },
        {
          src: require('../assets/images/img8.jpg'),
        },
        {
          src: require('../assets/images/img9.jpg'),
        },
        {
          src: require('../assets/images/img10.jpg'),
        },
        {
          src: require('../assets/images/img11.jpg'),
        },
        {
          src: require('../assets/images/img12.jpg'),
        },
        {
          src: require('../assets/images/img13.jpg'),
        },
        {
          src: require('../assets/images/img14.jpg'),
        },
      ],
    }
  },
}
</script>

<style></style>
