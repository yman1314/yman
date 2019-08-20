<template>
  <section class="ym-main">
    <ul>
      <li>
        <a href="#bg1"></a>
      </li>
      <li>
        <a href="#bg2"></a>
      </li>
      <li>
        <a href="#bg3"></a>
      </li>
      <li>
        <a href="#bg4"></a>
      </li>
      <li>
        <a href="#bg5"></a>
      </li>
    </ul>
  </section>
</template>

<script>
export default {
  name: 'HelloWorld',
  props: {
    msg: String
  }
}
</script>

<style lang="scss">
.ym-main{
  position: absolute;
  width: 100%;
  height: 200px;
  bottom: 20vh;
  z-index: 4;
  ul{
    height: 100%;
    display: flex;
    flex-flow: wrap;
    padding: 0 10vh;
    box-sizing: border-box;
  }
  li{
    background-color: rgb(141, 137, 137);
    list-style-type: none;
    width: 16%;
    max-width: 200px;
    min-width: 160px;
    margin: 0 2%;
  }
  a{
    display: block;
    height: 100%;
  }
}
</style>
