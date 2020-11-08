<template>
  <v-toolbar app>
    <v-toolbar-title>{{ siteTitle }}</v-toolbar-title>
    <v-spacer />
    <v-toolbar-item>
      <v-btn
        v-for="item in menuItems"
        :key="item.title"
        flat
        :to="item.to"
        v-text="item.title"
      />
    </v-toolbar-item>
  </v-toolbar>
</template>

<script>
export default {
  data () {
    return {
      siteTitle: 'De Mortem Et Diabolum',
      sidebar: false,
      menuItems: [
        {
          icon: 'mdi-apps',
          title: 'Welcome',
          to: '/'
        },
        {
          icon: 'mdi-chart-bubble',
          title: 'Bands',
          to: '/bands'
        },
        {
          icon: 'mdi-chart-bubble',
          title: 'News',
          to: '/news'
        }
      ]
    }
  }
}
</script>
