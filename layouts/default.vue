<template>
<div>
    <app-header/>
    <div class="container mx-auto py-4">
      <Nuxt/>
    </div>
</div>
</template>

<script>
import AppHeader from '~/components/AppHeader.vue'
export default {
  components: { AppHeader },

}
</script>

<style>

</style>