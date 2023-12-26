<template>
    <div class="bg-black">
      <v-img src="/fundo.png" class="background-image" cover height="950"
        :class="smAndDown ? 'w-0 h-0 ma-0 pa-0' : ''" />
      <v-img src="/fundo.png" class="background-image" cover height="450"
        :class="smAndDown ? '' : 'w-0 h-0 ma-0 pa-0'" />
    </div>
  
    <v-app class="bg-terciary">
      <default-bar />
  
  
      <div class="font d-flex justify-center align-center mt-16">
        <h2>Destaques</h2>
      </div>
  
      <v-container class="d-flex justify-space-between mt-16">
        <v-card width="300" class="elevation-24 bg-black" :class="smAndDown ? 'w-0' : 'mr-5'">
          <v-img src="/colhersalada.png" height="300px" cover></v-img>
  
          <v-card-title>
            Kit Salada
          </v-card-title>
  
          <v-card-subtitle>
            <h2>R$ 70,00</h2>
          </v-card-subtitle>
  
          <v-btn class="mt-4 mb-2 ml-2 elevation-24 bg-grey" :class="smAndDown ? 'w-75' : ''">COMPRAR</v-btn>
        </v-card>
  
        <v-card width="300" class="elevation-24 bg-black" :class="smAndDown ? 'w-75 mr-1' : 'mr-5'">
          <v-img src="/colhertuco.png" height="300px" cover></v-img>
  
          <v-card-title>
            Kit Tuco
          </v-card-title>
  
          <v-card-subtitle>
            <h2>R$ 70,00</h2>
          </v-card-subtitle>
  
          <v-btn class="mt-4 mb-2 ml-2 bg-grey" :class="smAndDown ? 'w-75' : ''">COMPRAR</v-btn>
        </v-card>
  
        <v-card width="300" class="elevation-24 bg-black" :class="smAndDown ? 'w-75' : 'mr-5'">
          <v-img src="/pratossaturno.png" height="300px" cover></v-img>
  
          <v-card-title>
            Kit Saturno
          </v-card-title>
  
          <v-card-subtitle>
            <h2>R$ 65,00</h2>
          </v-card-subtitle>
  
          <v-btn class="mt-4 mb-2 mr-2 ml-2 bg-grey" :class="smAndDown ? 'w-75' : ''">COMPRAR</v-btn>
        </v-card>
  
        <v-card width="300" class="elevation-24 bg-black" :class="smAndDown ? 'w-0' : ''">
          <v-img src="/setsauce.png" height="300px" cover></v-img>
  
          <v-card-title>
            Kit Sauce
          </v-card-title>
  
          <v-card-subtitle>
            <h2>R$ 120,00</h2>
          </v-card-subtitle>
  
          <v-btn class="mt-4 mb-2 mr-2 ml-2 bg-grey">COMPRAR</v-btn>
        </v-card>
      </v-container>
  
      <v-container class="d-flex justify-space-between" :class="smAndDown ? '' : 'w-0 h-0'">
        <v-card width="300" class="elevation-24 bg-black" :class="smAndDown ? 'w-75' : 'w-0'">
          <v-img src="/setsauce.png" height="300px" cover></v-img>
  
          <v-card-title>
            Kit Sauce
          </v-card-title>
  
          <v-card-subtitle>
            <h2>R$ 120,00</h2>
          </v-card-subtitle>
  
          <v-btn class=" mt-4 mb-2 ml-2 bg-grey" :class="smAndDown ? 'w-75' : ''">COMPRAR</v-btn>
        </v-card>
  
        <v-card width="300" class="elevation-24 bg-black" :class="smAndDown ? 'w-75 ml-1' : 'w-0'">
          <v-img src="/colhersalada.png" height="300px" cover></v-img>
  
          <v-card-title>
            Kit Salada
          </v-card-title>
  
          <v-card-subtitle>
            <h2>R$ 70,00</h2>
          </v-card-subtitle>
  
          <v-btn class="mt-4 mb-2 mr-2 ml-2 bg-grey" :class="smAndDown ? 'w-75' : ''">COMPRAR</v-btn>
        </v-card>
  
      </v-container>
  
  
      <v-container class="d-flex justify-space-between">
        <v-card width="300" class="elevation-24 bg-black" :class="smAndDown ? 'w-0' : 'mr-5'">
          <v-img src="/kitcoquetel.png" height="300px" cover></v-img>
  
          <v-card-title>
            Kit Coquetel
          </v-card-title>
  
          <v-card-subtitle>
            <h2>R$ 250,00</h2>
          </v-card-subtitle>
  
          <v-btn class="mt-4 mb-2 ml-2 bg-grey">COMPRAR</v-btn>
        </v-card>
  
        <v-card width="300" class="elevation-24 bg-black" :class="smAndDown ? 'w-75' : 'mr-5'">
          <v-img src="/tabuadark.png" height="300px" cover></v-img>
  
          <v-card-title>
            Tábua Dark
          </v-card-title>
  
          <v-card-subtitle>
            <h2>R$ 150,00</h2>
          </v-card-subtitle>
  
          <v-btn class="mt-4 mb-2 ml-2 bg-grey" :class="smAndDown ? 'w-75' : ''">COMPRAR</v-btn>
        </v-card>
  
        <v-card width="300" class="elevation-24 bg-black" :class="smAndDown ? 'w-75 ml-1' : 'mr-5'">
          <v-img src="/kitsaturno2.png" height="300px" cover></v-img>
  
          <v-card-title>
            Kit Dark
          </v-card-title>
  
          <v-card-subtitle>
            <h2>R$ 50,00</h2>
          </v-card-subtitle>
  
          <v-btn class="mt-4 mb-2 mr-2 ml-2 bg-grey" :class="smAndDown ? 'w-75' : ''">COMPRAR</v-btn>
        </v-card>
  
        <v-card width="300" class="elevation-24 bg-black" :class="smAndDown ? 'w-0' : ''">
          <v-img src="/tigelamamba.png" height="300px" cover></v-img>
  
          <v-card-title>
            Tigela Mamba
          </v-card-title>
  
          <v-card-subtitle>
            <h2>R$ 50,00</h2>
          </v-card-subtitle>
  
          <v-btn class="mt-4 mb-2 mr-2 ml-2 bg-grey">COMPRAR</v-btn>
        </v-card>
      </v-container>
  
      <v-container class="d-flex justify-space-between" :class="smAndDown ? '' : 'w-0 h-0'">
        <v-card width="300" class="elevation-24 bg-black" :class="smAndDown ? 'w-75' : 'w-0'">
          <v-img src="/kitcoquetel.png" height="300px" cover></v-img>
  
          <v-card-title>
            Kit Coquetel
          </v-card-title>
  
          <v-card-subtitle>
            <h2>R$ 250,00</h2>
          </v-card-subtitle>
  
          <v-btn class="mt-4 mb-2 ml-2 bg-grey" :class="smAndDown ? 'w-75' : ''">COMPRAR</v-btn>
        </v-card>
  
        <v-card width="300" class="elevation-24 bg-black" :class="smAndDown ? 'w-75 ml-1' : 'w-0'">
          <v-img src="/tigelamamba.png" height="300px" cover></v-img>
  
          <v-card-title>
            Tigela Mamba
          </v-card-title>
  
          <v-card-subtitle>
            <h2>R$ 50,00</h2>
          </v-card-subtitle>
  
          <v-btn class="mt-4 mb-2 mr-2 ml-2 bg-grey" :class="smAndDown ? 'w-75' : ''">COMPRAR</v-btn>
        </v-card>
      </v-container>
  
      <div :class="smAndDown ? 'mt-10 pt-10' : 'w-0 h-0'">
        <v-img src="/foto1.png" cover :class="smAndDown ? ' w-100' : 'w-0 h-0 pa-0 ma-0'" />
      </div>
  
      <div>
        <v-img src="/foto2.png" cover :class="smAndDown ? 'w-100 mb-10 pb-10' : 'w-0 h-0 pa-0 ma-0'" />
      </div>
  
      <div class="d-flex justify-space-between" :class="smAndDown ? 'w-0 h-0 pa-0 ma-0' : 'mt-10'">
        <v-parallax src="/foto1.png" class="mr-2" cover :class="smAndDown ? 'w-0 h-0 pa-0 ma-0' : ''" />
        <v-parallax src="/foto2.png" class="ml-2" cover :class="smAndDown ? 'w-0 h-0 pa-0 ma-0' : ''" />
      </div>
  
      <v-divider class="mt-10" />
  
      <default-view />
    </v-app>
  </template>
  
  <style scoped>
  .font {
    font-family: 'Plus Jakarta Sans', sans-serif;
    opacity: 0.8;
  }
  
  .img {
    opacity: 0.8;
  }
  </style>
  
  
  <script setup>
  import DefaultBar from './AppBar.vue'
  import DefaultView from './View.vue'
  import { useDisplay } from 'vuetify';
  
  const { smAndDown } = useDisplay()
  </script>
  