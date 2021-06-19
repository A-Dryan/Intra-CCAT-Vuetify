<template>
  <v-card height="100%">
    <v-navigation-drawer
      absolute
      permanent
      left
    >
      <template v-slot:prepend>
        <v-list-item two-line>
          <v-list-item-avatar>
            <img src="https://lh3.googleusercontent.com/proxy/DLIzw1_3DgbqL9vVcTt9krfmO1bOuqggTBXxTwDUnubmlbDhjMSfiYNvf9MinaL5N1XedCavKkZUOIETBMCjS1H6Q5pByIimLJL_IdjcrVYMzj-k7RCd3gnfZG41zRbH">
          </v-list-item-avatar>

          <v-list-item-content>
            <v-list-item-title>C C A T</v-list-item-title>
            <v-list-item-subtitle>Centro Cultural Avanzada Tecnologica</v-list-item-subtitle>
          </v-list-item-content>
        </v-list-item>
      </template>

      <v-divider></v-divider>

      <v-list dense>
        <v-list-item
          v-for="item in items"
          :key="item.title"
          :href="item.link"
        >
          <v-list-item-icon>
            <v-icon>{{ item.icon }}</v-icon>
          </v-list-item-icon>

          <v-list-item-content>
            <v-list-item-title>{{ item.title }}</v-list-item-title>
          </v-list-item-content>
        </v-list-item>
      </v-list>
      <v-btn
      color="red"
      to="/"
      block>
          Logout
      </v-btn>
    </v-navigation-drawer>
  </v-card>
</template>

<script>
  export default {
    data () {
      return {
        items: [
          { title: 'Home', icon: 'mdi-home-city', link: '#'},
          { title: 'Nosotros', icon: 'mdi-account', link: '#'},
          { title: 'Miembros', icon: 'mdi-account-group-outline', link: '#'},
          { title: 'Proyectos', icon: 'mdi-book-open-outline', link: '#'},
          { title: 'Direccion/Gerencia', icon: 'mdi-briefcase-account-outline', link: '#'},
          { title: 'Proximos Eventos', icon: 'mdi-calendar-star', link: '#'},
          { title: 'Productos', icon: 'mdi-cart-arrow-down', link: '#'},
        ],
      }
    },
  }
</script>