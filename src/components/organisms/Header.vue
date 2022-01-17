<template>
  <header ref="header" >
    <NavBar v-bind="$attrs" />
  </header>
  
  <div class="button" ref="button">
    <ButtonNavBar v-bind="$attrs" />
  </div>


  
</template>

<script>
import { ref, onMounted} from "vue";
import { NavBar } from "../molecules/";
import {ButtonNavBar} from '../atoms'
export default {
  components: {
    NavBar,
   ButtonNavBar
  },
  setup() {
    const header = ref(null);
    const button = ref(null);

    window.onscroll = () => {
      scrollFunction();
    };




    const scrollFunction = () => {
      if (document.body.scrollTop > 500 || document.documentElement.scrollTop > 500) {
        header.value.style.display = "none";
         button.value.style.display = "block";
      } else {
        header.value.style.display = "block";
        button.value.style.display = "none";
      }
    };

    onMounted(() => {
      scrollFunction();

    });

    return { header, button };
  },
};
</script>

<style lang="scss" scoped>
header {
  width: 100%;
  height: 70px;
  display: flex;
  align-items: center;
  justify-content: center;
  max-width: 1100px;
  margin: 0 auto;
  position: fixed;
  left: 0;
  right: 0;
  margin-left: auto;
  margin-right: auto;
}
</style>