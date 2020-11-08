<template>
  <v-container>
    <v-row>
      <v-col v-for="(item, i) in items" :key="i" cols="12">
        <div>
          <v-card>
            <v-img :src="item.img" height="200px" />
            <v-card-title class="headline" v-text="item.title" />
            <v-card-subtitle v-text="item.teaser" />
          </v-card>
        </div>
      </v-col>
    </v-row>
  </v-container>
</template>

<script>
/**
 * reusable card component
 *
 * @param {Array of Objects} items
 * @param {Boolean} spliced to check if used in main or overview page
 * @param {String} type to specify use case -> like 'Bands' or 'News'
 */
export default {
  name: 'CardComponent',
  props: {
    items: { type: Array, default: Array },
    spliced: Boolean,
    type: { type: String, default: '' }
  }
}
</script>

<style>
</style>
