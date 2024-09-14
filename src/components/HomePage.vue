<template>
  <v-container>
    <v-row class="d-flex justify-center">
      <v-col cols="8" class="main d-none d-sm-flex justify-center align-center">
        <div class="main bg-white d-flex">
          <v-col cols="6" class="imgc d-flex pa-0">
            <v-img
              class="img"
              src="@/assets/image-product-desktop.jpg"
              width="100"
              cover
            ></v-img>
          </v-col>
          <v-col
            cols="6"
            class="content d-flex flex-column justify-center align-center"
          >
            <v-col><div class="head mt-5">PERFUME</div></v-col>
            <v-col
              ><div class="title">Gabrielle Essence Eau De Parfum</div></v-col
            >
            <v-col
              ><div class="text">
                A floral, solar and voluptuous interpretation composed by
                Olivier Polge, Perfumer-Creator for the House of CHANEL.
              </div></v-col
            >
            <v-col class="mx-15"
              ><div class="price d-flex justify-start align-center">
                <div class="le mr-4">$149.99</div>
                <div class="ri">$169.99</div>
              </div></v-col
            >
            <v-col class=""
              ><v-btn
                block
                class="btn text-white text-capitalize"
                prepend-icon="mdi-cart-outline"
                flat
              >
                <template v-slot:prepend>
                  <v-icon class="text-white"></v-icon>
                </template>
                Add to Cart
              </v-btn></v-col
            >
          </v-col>
        </div>
      </v-col>
    </v-row>

    <div class="mobile pa-15 d-sm-none">
      <v-row class="">
        <v-img
          class="nwimg"
          src="@/assets/image-product-mobile.jpg"
          width="10"
          cover
        ></v-img>
      </v-row>

      <v-row class="bot bg-white">
        <v-col class="content d-flex flex-column justify-center align-center">
          <v-col><div class="head">PERFUME</div></v-col>
          <v-col
            ><div class="title">Gabrielle Essence Eau De Parfum</div></v-col
          >
          <v-col
            ><div class="text">
              A floral, solar and voluptuous interpretation composed by Olivier
              Polge, Perfumer-Creator for the House of CHANEL.
            </div></v-col
          >
          <v-col
            ><div class="price d-flex justify-start align-center">
              <div class="le mr-4">$149.99</div>
              <div class="ri">$169.99</div>
            </div></v-col
          >
          <v-col class=""
            ><v-btn
              block
              class="btn text-white text-capitalize"
              prepend-icon="mdi-cart-outline"
              flat
            >
              <template v-slot:prepend>
                <v-icon class="text-white"></v-icon>
              </template>
              Add to Cart
            </v-btn></v-col
          >
        </v-col>
      </v-row>
    </div>
  </v-container>
</template>

<script setup>
</script>

<style scoped>
@font-face {
  font-family: f1;
  src: url(@/assets/Fraunces_9pt-Bold.ttf);
}
.main {
  border-radius: 10px;
  
}
.imgc {
  width: 50%;
}
.img {
  /* Change width to 50% */
  width: 100%;
  border-top-left-radius: 10px; /* Top left corner */
  border-bottom-left-radius: 10px; /* Bottom left corner */
  border-top-right-radius: 0; /* No radius on the top right */
  border-bottom-right-radius: 0; /* No radius on the bottom right */
}
.nwimg {
  /* Change width to 50% */
  width: 10%;
  border-top-left-radius: 10px; /* Top left corner */
  border-bottom-left-radius: 0px; /* Bottom left corner */
  border-top-right-radius: 10px; /* No radius on the top right */
  border-bottom-right-radius: 0; /* No radius on the bottom right */
}
.mobile {
  transform: scale(1); /* Scales down to 50% of the original size */
  transform-origin: center; /* Controls where the scaling starts from */
}
.bot {
  border-bottom-left-radius: 10px; /* Bottom left corner */
  border-bottom-right-radius: 10px; /* No radius on the bottom right */
}
.head {
  color: #81838f;
  font-size: 10px;
  letter-spacing: 5px;
}

.title {
  color: #22272b;
  font-size: 25px;
  font-family: f1;
  line-height: 25px;
}
.text {
  color: #81838f;
  font-size: 14px;
  line-height: 18px;
}
.le {
  font-size: 28px;
  font-family: f1;
  color: #44836c;
}
.ri {
  text-decoration: line-through;
  color: #70727b;
  font-size: 12px;
}
.btn {
  background-color: #44836c;
}
.btn:hover {
  background-color: #1a4031;
}
.abc {
  border: 3px solid brown;
}
</style>
