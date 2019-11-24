<template>
  <site-template>
    <publicar-conteudo-vue />

    <card-conteudo-vue
      perfil="https://media.licdn.com/dms/image/C4E03AQFdBs73Y6RnsA/profile-displayphoto-shrink_200_200/0?e=1578528000&v=beta&t=5u-1vpV6NzhVsEK_jFcf-N4ZUqqcYpJn2V1txX2S9y8"
      data="03/11/2019 14:19"
      usuario="Marcos Gray"
    >
      <card-detalhe-vue
        img="https://materializecss.com/images/sample-1.jpg"
        titulo="Lago e montanhas"
        descricao="Um lago em um lugar belíssimo, com montanhas parcialmente cobertas por neve, e belíssimos pinheiros."
      />
    </card-conteudo-vue>
  </site-template>
</template>

<script>
import SiteTemplate from "@/templates/SiteTemplate";
import CardConteudoVue from "@/components/social/CardConteudoVue";
import CardDetalheVue from "@/components/social/CardDetalheVue";
import PublicarConteudoVue from "@/components/social/PublicarConteudoVue";

export default {
  name: "Home",
  data() {
    return {};
  },
  components: {
    SiteTemplate,
    CardConteudoVue,
    CardDetalheVue,
    PublicarConteudoVue
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
</style>
