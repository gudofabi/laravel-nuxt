<template>
  <div class="flex w-full bg-blue-400 shadow-sm justify-between text-white px-4 py-4">
      <h1>Nuxt-Auth</h1>
      <ul class="flex">
          <template v-if="$auth.loggedIn">
            <li><a class="px-2" href="/dashboard">Dashboard</a></li>
            <li><a class="px-2 cursor-pointer" @click.prevent="func_logout">Logout</a></li>
          </template>
          <template v-else>
          <li><a class="px-2" href="/login">Login</a></li>
          </template>
      </ul>
  </div>
</template>

<script>
export default {
    methods: {
        async func_logout() {
            try {
               await this.$auth.logout();
            } catch (error) {
                console.log(error);
            }
        }
    }
}
</script>

<style lang="scss" scoped>

</style>