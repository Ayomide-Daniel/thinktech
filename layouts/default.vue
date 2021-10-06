<template>
  <div>
    <v-app id="app-wrapper">
      <v-main>
        <NavbarComponent /><SubscribeComponent />
        <v-container id="app-container">
          <router-view></router-view
        ></v-container>
        <FooterComponent />
      </v-main>
    </v-app>
  </div>
</template>
<script>
import NavbarComponent from '~/components/includes/NavbarComponent'
import SubscribeComponent from '~/components/includes/SubscribeComponent'
import FooterComponent from '~/components/includes/FooterComponent'
export default {
  name: 'Default',
  components: {
    NavbarComponent,
    SubscribeComponent,
    FooterComponent,
  },
}
</script>

<style scoped></style>
