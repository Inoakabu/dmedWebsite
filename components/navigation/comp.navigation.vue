<template>
  <v-toolbar app tile>
    <v-spacer />
    <v-toolbar-item>
      <v-btn
        v-for="item in menuItems"
        :key="item.title"
        exact
        :to="item.to"
        text
        :x-large="false ? item.type : 'x-large'"
        v-text="item.title"
      />
    </v-toolbar-item>
    <v-spacer />
  </v-toolbar>
</template>

<script>
export default {
  data () {
    return {
      menuItems: [
        {
          icon: 'mdi-chart-bubble',
          title: 'De Mortem Et Diabolum',
          to: '/',
          type: 'x-large'
        },
        {
          icon: 'mdi-chart-bubble',
          title: 'Bands',
          to: '/bands',
          type: 'small'
        },
        {
          icon: 'mdi-chart-bubble',
          title: 'News',
          to: '/news',
          type: 'small'
        }
      ]
    }
  }
}
</script>
