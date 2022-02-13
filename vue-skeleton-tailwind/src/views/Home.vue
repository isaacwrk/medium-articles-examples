<template>
  <Page>
    
  </Page>

</template>

<script lang="ts">
import { Options, Vue } from 'vue-class-component';
import Page from '@/components/Page.vue'
import Card from '@/components/Card.vue'
import Skeleton from "@/components/Skeleton.vue"

@Options({
  components: {
    Page,
    Card,
    Skeleton
  },
})
export default class Home extends Vue {}
</script>
