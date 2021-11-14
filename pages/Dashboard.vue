<template>
    <div class="container mx-auto">
        <div class="bg-white p-4 shadow-md rounded-xl mx-auto">
            <h1 class="text-blue-400 font-semibold text-2xl mb-2">Private dashboard</h1>
            <p>Welcome {{ $auth.user.name }}</p>
            <p>This page can be access just only of authenticated user</p>
        </div>
    </div>
</template>

<script>
export default {
    middleware: "auth"
}
</script>

<style>

</style>