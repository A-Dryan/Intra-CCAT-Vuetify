<template>
<v-row style="height: 100%; width: 100%">
  <v-col cols="3">
   <MenuInterface/>
  </v-col>
  <v-col cols="9" class="mt-4">
  <EditorSlideHome/>
  </v-col>
</v-row>
</template>

<script>
  import MenuInterface from '../components/MenuInterface'
  import EditorSlideHome from '../components/EditorSlideHome'

  export default {
    name: 'modHome',

     components: {
      MenuInterface,
      EditorSlideHome,
    },
  }
</script>
