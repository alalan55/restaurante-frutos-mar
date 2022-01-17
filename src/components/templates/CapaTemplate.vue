<template>
  <section class="capa-template">
    <div class="conteudo-capa">
      <Header class="navbar" />
    </div>
  </section>
</template>

<script>
import { Header } from "@/components/organisms";
export default {
  components: {
    Header,
  },
};
</script>

<style lang="scss" scoped>
.capa-template {
  height: 100vh;
  background: url(https://images.pexels.com/photos/1483780/pexels-photo-1483780.jpeg?auto=compress&cs=tinysrgb&h=750&w=1260) no-repeat;
  background-size: cover;
  width: 100%;
  .conteudo-capa{
      margin-top: none;
      border: 1px solid none;
      height: 100%;
      padding: 2.5rem .8rem;
  }
}
</style>