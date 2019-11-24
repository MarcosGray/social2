<template>
  <nav :class="cor || 'purple darken-4'">
    <div class="nav-wrapper container">
      <a :href="url || '#/'" class="brand-logo">
        <i class="material-icons">cloud</i>
        {{logo || 'Site'}}
      </a>
      <ul id="nav-mobile" class="right hide-on-med-and-down">
        <slot />
      </ul>
    </div>
  </nav>
</template>

<script>
export default {
  name: "NavBarVue",
  props: ["logo", "url", "cor"],
  data() {
    return {};
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
</style>
