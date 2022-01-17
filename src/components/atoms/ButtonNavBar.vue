<template>
  <div class="btn">
    <svg
      xmlns="http://www.w3.org/2000/svg"
      class="icon icon-tabler icon-tabler-menu"
      width="44"
      height="44"
      viewBox="0 0 24 24"
      stroke-width="1.5"
      stroke="#000"
      fill="none"
      stroke-linecap="round"
      stroke-linejoin="round"
    >
      <path stroke="none" d="M0 0h24v24H0z" fill="none" />
      <line x1="4" y1="8" x2="20" y2="8" />
      <line x1="4" y1="16" x2="20" y2="16" />
    </svg>
  </div>
</template>

<script>
export default {};
</script>

<style lang="scss" scoped>
.btn {
  background: white;
  position: fixed;
  top: 45px;
  left: 25px;
  width: 45px;
  height: 45px;
  display: flex;
  align-items: center;
  justify-content: center;
  cursor: pointer;
  border-radius: 50%;
   -webkit-box-shadow: 2px 3px 8px -3px rgba(0, 0, 0, 0.34);
  box-shadow: 2px 3px 8px -3px rgba(0, 0, 0, 0.34);


  .icon{
    //   width: 70%;
    width: 30px;
  }
}
</style>