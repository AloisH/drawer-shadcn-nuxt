<script setup lang="ts">
const route = useRoute()
</script>

<template>
  <div>
    <h1>Nuxt Routing set up successfully!</h1>
    <p>Current route: {{ route.path }}</p>
    <a href="https://nuxt.com/docs/getting-started/routing" target="_blank">Learn more about Nuxt Routing</a>
  </div>
  <div>
    <Drawer>
      <DrawerTrigger as-child>
        <Button class="h-32 text-lg w-full">+ New word family</Button>
      </DrawerTrigger>
      <DrawerContent class="pb-32 px-4">
        <DrawerHeader>
          <DrawerTitle>
            Family
          </DrawerTitle>
          <DrawerDescription>Add a new family</DrawerDescription>
        </DrawerHeader>
      </DrawerContent>
    </Drawer>
  </div>
</template>

<style>
@import url("~/assets/css/tailwind.css");
</style>
