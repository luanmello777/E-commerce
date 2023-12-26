<template>
  <v-main>
    <div class="font d-flex justify-center align-center" :class="smAndDown ? '' : 'mt-5'">
      <h2 class="font">Lançamentos</h2>
    </div>

    <v-container class="d-flex justify-space-between mt-16">
      <v-card width="300" class="elevation-24 bg-black" :class="smAndDown ? 'w-0' : 'mr-5'">
        <v-img src="/tigelafavo.png" height="300px" cover></v-img>

        <v-card-title>
          Tigela Favo
        </v-card-title>

        <v-card-subtitle>
          <h2>R$ 50,00</h2>
        </v-card-subtitle>

        <v-btn class="mt-4 mb-2 ml-2 elevation-24 bg-grey" :class="smAndDown ? 'w-75' : ''">COMPRAR</v-btn>
      </v-card>

      <v-card width="300" class="elevation-24 bg-black" :class="smAndDown ? 'w-0 h-0' : 'mr-5'">
        <v-img src="/travessasaturno.png" height="300px" cover></v-img>

        <v-card-title>
          Travessa Saturno
        </v-card-title>

        <v-card-subtitle>
          <h2>R$ 80,00</h2>
        </v-card-subtitle>

        <v-btn class="mt-4 mb-2 ml-2 bg-grey" :class="smAndDown ? 'w-75' : ''">COMPRAR</v-btn>
      </v-card>

      <v-card width="300" class="elevation-24 bg-black" :class="smAndDown ? 'w-75 mr-1' : 'w-0 h-0'">
        <v-img src="/travessasaturno.png" height="300px" cover></v-img>

        <v-card-title>
          Trave. Saturno
        </v-card-title>

        <v-card-subtitle>
          <h2>R$ 80,00</h2>
        </v-card-subtitle>

        <v-btn class="mt-4 mb-2 ml-2  bg-grey" :class="smAndDown ? 'w-75' : ''">COMPRAR</v-btn>
      </v-card>

      <v-card width="300" class="elevation-24 bg-black" :class="smAndDown ? 'w-75' : 'mr-5'">
        <v-img src="/tigelaclean.png" height="300px" cover></v-img>

        <v-card-title>
          Tigela Clean
        </v-card-title>

        <v-card-subtitle>
          <h2>R$ 50,00</h2>
        </v-card-subtitle>

        <v-btn class="mt-4 mb-2 mr-2 ml-2  bg-grey" :class="smAndDown ? 'w-75' : ''">COMPRAR</v-btn>
      </v-card>

      <v-card width="300" class="elevation-24 bg-black" :class="smAndDown ? 'w-0' : ''">
        <v-img src="/travessadark.png" height="300px" cover></v-img>

        <v-card-title>
          Travessa Dark
        </v-card-title>

        <v-card-subtitle>
          <h2>R$ 170,00</h2>
        </v-card-subtitle>

        <v-btn class="mt-4 mb-2 mr-2 ml-2  bg-grey">COMPRAR</v-btn>
      </v-card>
    </v-container>

    <v-container class="d-flex justify-space-between" :class="smAndDown ? '' : 'w-0 h-0'">
      <v-card width="300" class="elevation-24 bg-black" :class="smAndDown ? 'w-75' : 'w-0'">
        <v-img src="/travessadark.png" height="300px" cover></v-img>

        <v-card-title>
          Trave. Dark
        </v-card-title>

        <v-card-subtitle>
          <h2>R$ 170,00</h2>
        </v-card-subtitle>

        <v-btn class=" mt-4 mb-2 ml-2 bg-grey" :class="smAndDown ? 'w-75' : ''">COMPRAR</v-btn>
      </v-card>

      <v-card width="300" class="elevation-24 bg-black" :class="smAndDown ? 'w-75 ml-1' : 'w-0'">
        <v-img src="/tigelafavo.png" height="300px" cover></v-img>

        <v-card-title>
          Tigela Favo
        </v-card-title>

        <v-card-subtitle>
          <h2>R$ 50,00</h2>
        </v-card-subtitle>

        <v-btn class="mt-4 mb-2 mr-2 ml-2 bg-grey" :class="smAndDown ? 'w-75' : ''">COMPRAR</v-btn>
      </v-card>

    </v-container>

    <v-divider class="mt-10" />

    <div>
      <v-img src="/fundo2.png" cover height="300" class="background-image" :class="smAndDown ? 'mt-16 h-75' : ''" />
    </div>

    <v-container class="mt-16 pt-16">
      <h2 class="font d-flex justify-center align-center" :class="smAndDown ? '' : ''">Since 1999</h2>
      <p class="d-flex justify-center align-center" :class="smAndDown ? '' : 'mt-2'">Há mais de 20 anos decorando sua
        casa</p>
    </v-container>

    <div class="d-flex justify-center align-center" :class="smAndDown ? 'mt-8' : 'mt-5'">
      <v-btn class="bg-transparent border-rounded text-white elevation-24" href="https://www.instagram.com/somosrio.home/"
        target="_about-blank"><svg-icon type="mdi" :path="path" class="mr-2"></svg-icon>Siga-nos</v-btn>
    </div>

    <v-divider class="mt-16" />



    <v-container :class="smAndDown ? 'mt-8' : 'mt-16 ml-16'">
      <p :class="smAndDown ? 'font1 ml-1 mb-5' : 'font1 ml-1 mb-3'">ASSINE NOSSA NEWSLETTER</p>

      <v-form>
        <v-row>
          <v-col cols="11" md="4">
            <v-text-field v-model="Email" :rules="emailRules" label="Email" placeholder="email@email.com.br"
              hint="Informe seu E-mail" color="white"></v-text-field>
            <v-btn class="bg-transparent border-rounded" :class="smAndDown ? '' : 'mt-2 mb-5'" type="submit">
              Assinar
            </v-btn>
          </v-col>
        </v-row>
      </v-form>
    </v-container>

    <v-container :class="smAndDown ? 'mt-10' : 'mt-16 ml-16'">
      <p>ENTRE EM CONTATO :</p>
      <p class="font mt-5"><svg-icon type="mdi" :path="path2" class="mr-3"></svg-icon>(21) 999999999</p>
      <p class="font mt-5"><svg-icon type="mdi" :path="path3" class="mr-3"></svg-icon>rio@nuvemshop.com</p>
      <p class="font mt-5"><svg-icon type="mdi" :path="path4" class="mr-3"></svg-icon>Alameda Vicente Pinzon, 173, São
        Paulo</p>
    </v-container>


    <div :class="smAndDown ? 'mt-16' : ''">
      <v-footer class="bg-black d-flex justify-center align-center mt-16">
        <p class="font1">Copyright 2023 - Todos os direitos reservados.</p>
      </v-footer>
    </div>


    <div class="bg-black w-100 d-flex align-center justify-center" :class="smAndDown ? 'mt-5' : 'mt-16'">
      <v-chip color="white" class=" mt-3 mb-3" href="https://github.com/luanmello777" target="_blank>"><svg-icon
          type="mdi" :path="path1" class="mr-2"></svg-icon>github.com/Luanmello777
      </v-chip>
    </div>

    <router-view />
  </v-main>
</template>

<style scoped>
.font {
  font-family: 'Plus Jakarta Sans', sans-serif;
  opacity: 0.8;
}

.font1 {
  font-family: 'Plus Jakarta Sans', sans-serif;
  opacity: 0.8;
  font-size: 13px;
}

.border-rounded {
  border-color: grey;
  border-width: 2px;
}
</style>


<script setup>
import { useDisplay } from 'vuetify';
import SvgIcon from '@jamescoyle/vue-icon';
import { mdiInstagram, mdiGithub, mdiCellphone, mdiEmail, mdiMapMarkerRadius } from '@mdi/js';
import { ref } from 'vue';


const { smAndDown } = useDisplay()
const path = mdiInstagram;
const path1 = mdiGithub;
const path2 = mdiCellphone;
const path3 = mdiEmail;
const path4 = mdiMapMarkerRadius;

const Email = ref('');
const emailRules = ref([
  value => {
    if (value) return true;
    return 'É necessário inserir um E-mail.';
  },
  value => {
    if (/.+@.+\..+/.test(value)) return true;
    return 'E-mail deve ser válido.';
  },
]);
</script>
