<template>
  <Loader :load="isLoading"/>
  <NuxtLayout>
    <NuxtPage/>
  </NuxtLayout>
</template>

<script setup>
  const isLoading = ref(true)
  onMounted(() => {
      isLoading.value = false
  })
</script>

