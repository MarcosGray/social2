<template  >
  <login-template>
    <h4>Login de Acesso</h4>
    <div class="row">
      <grid-vue class="input-field" tamanho="12">
        <input id="last_name" type="text" class="validate" />
        <label for="last_name">Seu e-mail</label>
      </grid-vue>
    </div>
    <div class="row">
      <grid-vue class="input-field" tamanho="12">
        <input id="password" type="password" class="validate" />
        <label for="password">Sua senha</label>
      </grid-vue>
    </div>
    <button type="submit" class="btn">Entrar</button>
    <button type="submit" class="btn orange">Cadastre-se</button>
  </login-template>
</template>

<script>
import LoginTemplate from "@/templates/LoginTemplate";
import GridVue from "@/components/layout/GridVue";

export default {
  name: "Login",
  data() {
    return {};
  },
  components: {
    LoginTemplate,
    GridVue
  }
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
</style>
