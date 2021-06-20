<template>
<v-container>
  <v-card
    class="mx-auto"
    max-width="700"
    max-height="200"
  >
  <v-form>
    <v-row>
    <v-col cols="4">
    <v-img
    contain
      class="white--text align-center"
      height="200px"
      src="https://www.kelea.es/ETG_wp-content/uploads/2020/09/metodologia-scrum-agile.jpg"
    >
    </v-img>
    </v-col>
    <v-col cols="8">
     <v-text-field class="mx-2 ml-10">
        <template v-slot:label>
         introduce el <strong>Url</strong> Aqui <v-icon style="vertical-align: middle">
            mdi-file-find
          </v-icon>
        </template>
      </v-text-field>
    <v-file-input
    multiple
    label="Imagen"
    class="mx-2"
  ></v-file-input>
          <div class="mx-3" style="display: flex; justify-content: flex-end;">
            <v-btn
              color="error"
              fab
              dark
            >
              <v-icon>mdi-delete</v-icon>
            </v-btn>
          </div>
    </v-col>
    </v-row>
  </v-form>
  </v-card>
</v-container>
</template>
