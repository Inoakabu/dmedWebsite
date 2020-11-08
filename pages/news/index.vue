<template>
  <v-container>
    <v-row>
      <v-col cols="12">
        <div>
          <CardComp :items="news" />
        </div>
      </v-col>
    </v-row>
  </v-container>
</template>

<script>
import CardComp from '@/components/structure/reusable/comp.cards.vue'
export default {
  name: 'NewsList',
  components: {
    CardComp
  },
  data () {
    return {
      news: [
        {
          title: 'News 1',
          teaser: 'Teaser 1',
          img: 'https://dmed-cockpit.cl.semicode.de/storage/uploads/2020/02/10/5e411c496248fdmed2020_web_band_misyrming.png'
        },
        {
          title: 'News 2',
          teaser: 'Teaser 2',
          img: 'https://dmed-cockpit.cl.semicode.de/storage/uploads/2020/02/10/5e411c496248fdmed2020_web_band_misyrming.png'
        },
        {
          title: 'News 3',
          teaser: 'Teaser 3',
          img: 'https://dmed-cockpit.cl.semicode.de/storage/uploads/2020/02/10/5e411c496248fdmed2020_web_band_misyrming.png'
        },
        {
          title: 'News 4',
          teaser: 'Teaser 4',
          img: 'https://dmed-cockpit.cl.semicode.de/storage/uploads/2020/02/10/5e411c496248fdmed2020_web_band_misyrming.png'
        }
      ]
    }
  }
}
</script>

<style>

</style>
