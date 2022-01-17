<template>
  <nav>
    <div class="logo">
      <span> Lag.</span>
    </div>

    <ul class="itens">
      <li class="item"><a href="#sobre">Sobre</a></li>
      <li class="item"><a>Localização</a></li>
      <li class="item"><a>Menu</a></li>
      <li class="item"><a>Social</a></li>
    </ul>
  </nav>
</template>

<script>
export default {
  setup(){

    return{

    }
  }
};
</script>

<style lang="scss" scoped>
nav {
  background: white;
  width: 100%;
  margin: 0 auto;
  height: 100%;
  border-radius: 35px;

  display: flex;
  align-items: center;
  justify-content: space-between;
  padding: 0 1rem;
  -webkit-box-shadow: 2px 3px 8px -3px rgba(0, 0, 0, 0.34);
  box-shadow: 2px 3px 8px -3px rgba(0, 0, 0, 0.34);

  .logo {
    background: rgb(97, 203, 211);
    width: 70px;
    height: 40px;
    border-radius: 25px;
    display: flex;
    align-items: center;
    justify-content: center;
    color: white;
    span {
      font-weight: 700;
    }
  }

  .itens {
    padding: 0;
    display: flex;

    .item {
      list-style: none;
      margin: 0 0.5rem;
      padding: 0;
      cursor: pointer;
      transition: 0.2s ease-in-out;

      a {
        font-weight: 400;
        color: rgb(44, 44, 44);
        text-decoration: none;

        &:hover {
          color: rgb(122, 122, 122);
        }
      }
    }
  }
}
</style>