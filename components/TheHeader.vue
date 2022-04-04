<template>
  <div class="header">
    <h1 class="font-bold text-blue-400 text-4xl pl-3 pt-3 pb-0">
      <slot></slot>
    </h1>
    <TheNavigation />
  </div>
</template>
<style scoped>
.header {
  width: 80%;
  padding-bottom:0;
}
</style>