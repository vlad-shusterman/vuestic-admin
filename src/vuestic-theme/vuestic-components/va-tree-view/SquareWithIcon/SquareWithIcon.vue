<template>
  <div class="square-with-icon">
    <va-icon :icon="iconClass"/>
  </div>
</template>

<script>
export default {
  name: 'square-with-icon',
  props: {
    iconClass: {
      type: String,
      required: true,
    },
  },
}
</script>

<style lang="scss">
@import "../../../vuestic-sass/resources/resources";

.square-with-icon {
  @include flex-center();
  align-items: center;
  border-radius: 0.1875rem;
  height: 1.375rem;
  width: 1.375rem;
  color: $white;
  background-color: $vue-green;
}
</style>
