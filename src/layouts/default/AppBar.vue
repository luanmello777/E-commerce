<template>
  <v-app-bar height="100" :class="smAndDown ? 'bg-transparent' : 'bg-transparent'">
    <div :class="smAndDown ? 'w-25 mt-2 pr-2' : ''">
      <v-img src="/logo.png" class="ml-8" width="150" />
    </div>

    <div class="d-flex justify-space-between" :class="smAndDown ? 'w-0 h-0 pt-16 mt-16' : 'ml-10 mt-1'">
      <v-dialog transition="dialog-bottom-transition" width="auto" :class="smAndDown ? 'w-0 h-0 pa-0 ma-0' : ''">
        <template v-slot:activator="{ props }">
          <v-btn color="primary" v-bind="props" class="font">Utensilios</v-btn>
        </template>
        <template v-slot:default="{ isActive }">
          <v-card class="bg-black">
            <v-toolbar color="secondary"></v-toolbar>
            <v-card-text>
              <div>
                <v-img src="/tabuadark.png" width="500" />
                <p class="mt-3 d-flex justify-center">Tábua Dark</p>
                <v-chip class="mt-3 d-flex justify-center ml-15 w-75">R$ 150,00</v-chip>
                <v-btn class="mb-10 mt-3 ml-2 w-100">COMPRAR</v-btn>
                <v-img src="/kitsaturno2.png" width="500" />
                <p class="mt-3 d-flex justify-center">Kit Dark</p>
                <v-chip class="mt-3 d-flex justify-center ml-15 w-75">R$ 50,00</v-chip>
                <v-btn class="mb-10 mt-3 ml-2 w-100">COMPRAR</v-btn>
                <v-img src="/setsauce.png" width="500" />
                <p class="mt-3 d-flex justify-center">Kit Sauce</p>
                <v-chip class="mt-3 d-flex justify-center ml-15 w-75">R$ 120,00</v-chip>
                <v-btn class="mb-10 mt-3 ml-2 w-100">COMPRAR</v-btn>
                <v-img src="/colhertuco.png" width="500" />
                <p class="mt-3 d-flex justify-center">Kit Tuco</p>
                <v-chip class="mt-3 d-flex justify-center ml-15 w-75">R$ 70,00</v-chip>
                <v-btn class="mb-10 mt-3 ml-2 w-100">COMPRAR</v-btn>
                <v-img src="/colhersalada.png" width="500" />
                <p class="mt-3 d-flex justify-center">Kit Salada</p>
                <v-chip class="mt-3 d-flex justify-center ml-15 w-75">R$ 70,00</v-chip>
                <v-btn class="mb-10 mt-3 ml-2 w-100">COMPRAR</v-btn>
              </div>
            </v-card-text>
            <v-card-actions class="justify-end">
              <v-btn class="bg-grey" variant="text" @click="isActive.value = false">Fechar</v-btn>
            </v-card-actions>
          </v-card>
        </template>
      </v-dialog>

      <v-dialog transition="dialog-bottom-transition" width="auto">
        <template v-slot:activator="{ props }">
          <v-btn color="primary" v-bind="props" class="font">Louças</v-btn>
        </template>
        <template v-slot:default="{ isActive }">
          <v-card class="bg-black">
            <v-toolbar color="secondary"></v-toolbar>
            <v-card-text>
              <div>
                <v-img src="/pratossaturno.png" width="500" />
                <p class="mt-3 d-flex justify-center">Kit Saturno</p>
                <v-chip class="mt-3 d-flex justify-center ml-15 w-75">R$ 65,00</v-chip>
                <v-btn class="mb-10 mt-3 ml-2 w-100">COMPRAR</v-btn>
                <v-img src="/travessadark.png" width="500" />
                <p class="mt-3 d-flex justify-center">Travessa Dark</p>
                <v-chip class="mt-3 d-flex justify-center ml-15 w-75">R$ 170,00</v-chip>
                <v-btn class="mb-10 mt-3 ml-2 w-100">COMPRAR</v-btn>
                <v-img src="/tigelaclean.png" width="500" />
                <p class="mt-3 d-flex justify-center">Tigela Clean</p>
                <v-chip class="mt-3 d-flex justify-center ml-15 w-75">R$ 50,00</v-chip>
                <v-btn class="mb-10 mt-3 ml-2 w-100">COMPRAR</v-btn>
                <v-img src="/travessasaturno.png" width="500" />
                <p class="mt-3 d-flex justify-center">Travessa Saturno</p>
                <v-chip class="mt-3 d-flex justify-center ml-15 w-75">R$ 80,00</v-chip>
                <v-btn class="mb-10 mt-3 ml-2 w-100">COMPRAR</v-btn>
                <v-img src="/tigelafavo.png" width="500" />
                <p class="mt-3 d-flex justify-center">Tigela Favo</p>
                <v-chip class="mt-3 d-flex justify-center ml-15 w-75">R$ 50,00</v-chip>
                <v-btn class="mb-10 mt-3 ml-2 w-100">COMPRAR</v-btn>
                <v-img src="/tigelamamba.png" width="500" />
                <p class="mt-3 d-flex justify-center">Tigela Mamba</p>
                <v-chip class="mt-3 d-flex justify-center ml-15 w-75">R$ 50,00</v-chip>
                <v-btn class="mb-10 mt-3 ml-2 w-100">COMPRAR</v-btn>
              </div>
            </v-card-text>
            <v-card-actions class="justify-end">
              <v-btn class="bg-grey" variant="text" @click="isActive.value = false">Fechar</v-btn>
            </v-card-actions>
          </v-card>
        </template>
      </v-dialog>

      <v-dialog transition="dialog-bottom-transition" width="auto">
        <template v-slot:activator="{ props }">
          <v-btn color="primary" v-bind="props" class="font">Coqueteleira</v-btn>
        </template>
        <template v-slot:default="{ isActive }">
          <v-card class="bg-black">
            <v-toolbar class="ml-10" color="secondary"></v-toolbar>
            <v-card-text>
              <div>
                <v-img src="/kitcoquetel.png" width="500" />
                <p class="mt-3 d-flex justify-center">Kit Coquetel</p>
                <v-chip class="mt-3 d-flex justify-center ml-15 w-75">R$ 250,00</v-chip>
                <v-btn class="mb-10 mt-3 ml-2 w-100">COMPRAR</v-btn>
                <v-img src="/coqueteleira.png" width="500" />
                <p class="mt-3 d-flex justify-center">Coqueteleira</p>
                <v-chip class="mt-3 d-flex justify-center ml-15 w-75">R$ 80,00</v-chip>
                <v-btn class="mb-10 mt-3 ml-2 w-100">COMPRAR</v-btn>
              </div>
            </v-card-text>
            <v-card-actions class="justify-end">
              <v-btn class="bg-grey" variant="text" @click="isActive.value = false">Fechar</v-btn>
            </v-card-actions>
          </v-card>
        </template>
      </v-dialog>
    </div>

    <v-app-bar-title />

    <div class="mr-5 d-flex justify-space-between">
      <v-dialog width="500">
        <template v-slot:activator="{ props }">
          <v-btn icon="mdi-magnify" v-bind="props" text="Open Dialog"> </v-btn>
        </template>
        <template v-slot:default="{ isActive }">
          <v-card class="bg-secondary">
            <v-card-text>
              <v-form>
                <v-row>
                  <v-col cols="12" md="12">
                    <v-text-field placeholder="O que você está buscando?" color="blue"></v-text-field>
                  </v-col>
                </v-row>
              </v-form>
            </v-card-text>
            <v-card-actions>
              <v-spacer></v-spacer>
              <v-btn class="bg-primary w-100 mb-5" text="Procurar" @click="isActive.value = false"></v-btn>
            </v-card-actions>
          </v-card>
        </template>
      </v-dialog>

      <v-dialog width="500" class="bg-black">
        <template v-slot:activator="{ props }">
          <v-btn icon="mdi-account" color="primary" v-bind="props"></v-btn>
        </template>
        <template v-slot:default="{ isActive }">
          <v-card title="CADASTRAR-SE">
            <v-card-text>
              <v-form v-model="valid">
                <v-container>
                  <v-row>
                    <v-col cols="12" md="10">
                      <v-text-field v-model="nome" :rules="nomeRules" label="Nome" color="blue" hint="Informe seu nome"
                        prepend-icon="mdi-account-circle-outline"></v-text-field>
                    </v-col>

                    <v-col cols="12" md="10">
                      <v-text-field v-model="Email" :rules="emailRules" label="Email" placeholder="email@email.com.br"
                        hint="Informe seu E-mail" color="blue" prepend-icon="mdi-email"></v-text-field>
                    </v-col>

                    <v-col cols="12" md="10">
                      <v-text-field v-model="Senha" :rules="senhaRules" label="Senha" color="blue"
                        hint="Informe sua senha" prepend-icon="mdi-form-textbox-password"></v-text-field>
                    </v-col>

                    <v-col cols="12" md="10">
                      <v-text-field v-model="RepitirSenha" :rules="repitirsenhaRules" label="Repitir Senha" color="blue"
                        hint="Informe sua senha novamente" prepend-icon="mdi-form-textbox-password"></v-text-field>
                    </v-col>
                  </v-row>
                </v-container>
                <v-checkbox v-model="checkbox" class="font2"
                  label="Li e concordo com os Termos de Uso e Política de Privacidade." required></v-checkbox>
              </v-form>

              <v-card-actions class="d-flex justify-center">
                <v-btn class="bg-black w-100" text="Cadastrar" @click="isActive.value = false"></v-btn>
              </v-card-actions>
            </v-card-text>
          </v-card>
        </template>
      </v-dialog>

      <v-dialog width="500">
        <template v-slot:activator="{ props }">
          <v-btn icon="mdi-cart" color="primary" v-bind="props" text="Open Dialog"> </v-btn>
        </template>
        <template v-slot:default="{ isActive }">
          <v-card title="CARRINHO DE COMPRAS" class="bg-black">
            <v-card-text>
              <v-chip class="d-flex justify-center align-center">O carrinho de compras está vazio.</v-chip>
            </v-card-text>
            <v-card-actions>
              <v-spacer></v-spacer>
              <v-btn class="bg-primary" text="Fechar" @click="isActive.value = false"></v-btn>
            </v-card-actions>
          </v-card>
        </template>
      </v-dialog>
    </div>
  </v-app-bar>
</template>

<style scoped>
.font {
  font-family: 'Plus Jakarta Sans', sans-serif;
  opacity: 0.8;
  font-size: 11px;
}
</style>

<script setup>
import { useDisplay } from 'vuetify';
import { ref } from 'vue';


const { smAndDown } = useDisplay()
const checkbox = ref(false);
const valid = ref(false);

const nome = ref('');
const nomeRules = ref([
  value => {
    if (value) return true;
    return 'É necessário inserir um Nome.';
  },
  value => {
    if (value?.length <= 50) return true;
    return 'Insira um nome de no minimo 3 letras.';
  },
]);

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

const Senha = ref('');
const senhaRules = ref([
  value => {
    if (value) return true;
    return 'É necessário inserir uma Senha.';
  },
  value => {
    if (/.+@.+\..+/.test(value)) return true;
    return 'A senha deve ser válida.';
  },
]);

const RepitirSenha = ref('');
const repitirsenhaRules = ref([
  value => {
    if (value) return true;
    return 'É necessário repitir a Senha.';
  },
  value => {
    if (/.+@.+\..+/.test(value)) return true;
    return 'A senha deve ser válida.';
  },
]);
</script>
