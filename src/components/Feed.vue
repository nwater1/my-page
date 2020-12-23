<template>
  <v-container class="no-pd-1">
    <v-row>
      <v-col cols="12" class="no-pd">
        <slot />
      </v-col>

      
    </v-row>

    
  </v-container>
</template>

<script>
  // Utilities
  import {
    mapState,
  } from 'vuex'

  export default {
    name: 'Feed',

    components: {
      FeedCard: () => import('@/components/FeedCard'),
    },

    data: () => ({
      layout: [2, 2, 1, 2, 2, 3, 3, 3, 3, 3, 3],
      page: 1,
    }),

    computed: {
      ...mapState(['articles']),
      pages () {
        return Math.ceil(this.articles.length / 11)
      },
      paginatedArticles () {
        const start = (this.page - 1) * 11
        const stop = this.page * 11

        return this.articles.slice(start, stop)
      },
    },

    watch: {
      page () {
        window.scrollTo(0, 0)
      },
    },
  }
</script>

<style scoped>
  .no-pd {
    padding-top: 0;
    padding-bottom: 0;
    padding-left: 0;
    padding-right: 0;
  }

  .no-pd-1 {
    padding-top: 0;
    padding-bottom: 0;
    padding-left: 1;
    padding-right: 1;
  }
</style>
