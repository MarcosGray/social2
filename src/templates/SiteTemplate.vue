<template>
  <span>
    <header>
      <nav-bar-vue logo="Social" url="#/" cor="light-blue darken-3">
        <li>
          <a href="#/">Home</a>
        </li>
        <li>
          <a href="#/login">Login</a>
        </li>
      </nav-bar-vue>
    </header>

    <main>
      <div class="container">
        <div class="row">
          <grid-vue tamanho="4">
            <card-menu-vue>
              <div class="row valign-wrapper">
                <grid-vue tamanho="4">
                  <img
                    src="https://media.licdn.com/dms/image/C4E03AQFdBs73Y6RnsA/profile-displayphoto-shrink_200_200/0?e=1578528000&v=beta&t=5u-1vpV6NzhVsEK_jFcf-N4ZUqqcYpJn2V1txX2S9y8"
                    alt
                    class="circle responsive-img"
                  />
                  <!-- notice the "circle" class -->
                </grid-vue>
                <grid-vue tamanho="8">
                  <span class="black-text">
                    <h5>Marcos Gray</h5>Desenvolvedor Full-stack na
                    <strong>Rentcars.com</strong>
                  </span>
                </grid-vue>
              </div>
            </card-menu-vue>
            <card-menu-vue>
              <h5>Bio Marcos Gray</h5>
            </card-menu-vue>
          </grid-vue>
          <grid-vue tamanho="8">
            <slot />
          </grid-vue>
        </div>
      </div>
    </main>

    <footer-vue
      logo="Social"
      cor="light-blue darken-3"
      descricao="Descrição da rede social"
      ano="2020"
    >
      <li>
        <a class="grey-text text-lighten-3" href="#!">Home</a>
      </li>
      <li>
        <a class="grey-text text-lighten-3" href="#!">Link 2</a>
      </li>
      <li>
        <a class="grey-text text-lighten-3" href="#!">Link 3</a>
      </li>
      <li>
        <a class="grey-text text-lighten-3" href="#!">Link 4</a>
      </li>
    </footer-vue>
  </span>
</template>

<script>
import NavBarVue from "@/components/layout/NavBarVue";
import FooterVue from "@/components/layout/FooterVue";
import GridVue from "@/components/layout/GridVue";
import CardMenuVue from "@/components/layout/CardMenuVue";

export default {
  name: "SiteTemplate",
  components: {
    NavBarVue,
    FooterVue,
    GridVue,
    CardMenuVue
  }
};
</script>

<style>
</style>
