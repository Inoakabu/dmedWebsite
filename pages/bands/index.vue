<template>
  <v-container>
    <v-row>
      <v-col cols="12">
        <div>
          <CardComp :items="bands" />
        </div>
      </v-col>
    </v-row>
  </v-container>
</template>

<script>
import CardComp from '@/components/structure/reusable/comp.cards.vue'
export default {
  name: 'BandList',
  components: {
    CardComp
  },
  data () {
    return {
      bands: [
        {
          title: 'Band 1',
          teaser: 'Teaser 1',
          img: 'https://dmed-cockpit.cl.semicode.de/storage/uploads/2020/02/10/5e411c496248fdmed2020_web_band_misyrming.png'
        },
        {
          title: 'Band 2',
          teaser: 'Teaser 2',
          img: 'https://dmed-cockpit.cl.semicode.de/storage/uploads/2020/02/10/5e411c496248fdmed2020_web_band_misyrming.png'
        },
        {
          title: 'Band 3',
          teaser: 'Teaser 3',
          img: 'https://dmed-cockpit.cl.semicode.de/storage/uploads/2020/02/10/5e411c496248fdmed2020_web_band_misyrming.png'
        },
        {
          title: 'Band 4',
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
