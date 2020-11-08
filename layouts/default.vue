<template>
  <v-app dark>
    <v-main>
      <NavComp />
      <v-container>
        <nuxt />
      </v-container>
    </v-main>
    <FooterComp />
  </v-app>
</template>

<script>
import NavComp from '@/components/navigation/comp.navigation.vue'
import FooterComp from '@/components/structure/site/comp.footer.vue'

export default {
  name: 'DefaultLayout',
  components: {
    NavComp,
    FooterComp
  },
  data () {
    return {
    }
  }
}
</script>
