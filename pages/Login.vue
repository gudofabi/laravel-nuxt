<template>
	<div>
		<a href="#" @click.prevent="func_login">Login</a>
	</div>
</template>

<script>
export default {
	middleware: ['guest'],	
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