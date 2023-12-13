<template>
  <div class="container flex items-center justify-cneter">
    <h1>Welcome</h1>
    <p>Sing in tu your profile</p>
    <button class="px-3 py-2 rounded-md bg-emerald-500 text-white inline-flex items-center">Sing In</button>
  </div>
</template>

<script lang="ts" setup>
  const userStore = useUserStore();

  const signIn =async () => {
    await userStore.signIn({
      username: 'kminchelle',
      password: '0lelplR',
    });

    await navigateTo('/profile',)
  }
</script>

<style>

</style>