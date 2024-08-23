<template>
    <div>
        <h2>About</h2>
        <p>Lorem ipsum dolor sit amet consectetur, adipisicing elit. Aliquid velit id ea consectetur maxime facere quis repellat provident temporibus voluptatem.</p>
        <p>Lorem ipsum dolor sit amet consectetur, adipisicing elit. Aliquid velit id ea consectetur maxime facere quis repellat provident temporibus voluptatem.</p>
        <p>{{ data }}</p>
    </div>
</template>

<script setup>

const { data } = await useFetch('/api/currency/NGN')

</script>

<style scoped>

h2 {
    margin-bottom: 20px;
    font-size: 36px;
  }
  p {
    margin: 20px 0;
  }

</style>