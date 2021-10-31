<template>
  <a href="#" @click.prevent="func_login">Login</a>
</template>

<script>
export default {
 methods: {
		func_login() {
			this.$auth.loginWith('laravelSanctum', {
				data: {
					email: 'godofredocpanel@gmail.com',
					password: 'password'
				}
			})
		}
	}
}
</script>

<style>

</style>