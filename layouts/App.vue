<template>
  <div id="app-layout">
    <div>
      <app-header v-show="showHeader"/>
    </div>
    <main>
      <nuxt />
    </main>
    <app-footer v-show="showFooter" />
  </div>
</template>

<script>
import AppHeader from '@/components/global/Header/AppHeader.vue';
import AppFooter from '@/components/global/Footer/AppFooter.vue';
export default {
  data(){
    return {

    }
  },
  components: {
    AppHeader,
    AppFooter
  },
  computed: {
    showFooter(){
      let pages = [];
      return pages.indexOf( this.$route.name ) == -1;
    },
    showHeader(){
      let pages = [];
      return pages.indexOf( this.$route.name ) == -1;
    },
  }
}
</script>
