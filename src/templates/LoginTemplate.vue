<template>
  <span>
    <main>
      <div class="container">
        <div class="row">
          <grid-vue style="margin-top:20%" tamanho="4">
            <card-menu-vue>
              <div class="row valign-wrapper">
                <grid-vue tamanho="12">
                  <slot />
                </grid-vue>
              </div>
            </card-menu-vue>
          </grid-vue>
        </div>
      </div>
    </main>
  </span>
</template>

<script>
import GridVue from "@/components/layout/GridVue";
import CardMenuVue from "@/components/layout/CardMenuVue";

export default {
  name: "LoginTemplate",
  components: {
    GridVue,
    CardMenuVue
  }
};
</script>

<style>
</style>
