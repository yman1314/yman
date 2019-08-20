<template>
  <section class="bg-img">
    <div class="bg a" id="bg1"></div>
    <div class="bg b" id="bg2"></div>
    <div class="bg c" id="bg3"></div>
    <div class="bg d" id="bg4"></div>
    <div class="bg e" id="bg5"></div>
  </section>
</template>

<script>
export default {
}
</script>

<style lang="scss">
.bg-img{
  position: absolute;
  overflow: hidden;
  z-index: 2;
  width: 100%;
  height: 100%;
  div.a{
    background:url(../assets/t4.jpg) no-repeat;
  }
  div.b{
    background:url(../assets/t6.jpg) no-repeat;
  }
  div.c{
    background:url(../assets/q3.jpg) no-repeat;
  }
  div.d{
    background:url(../assets/p8.jpg) no-repeat;
  }
  div.e{
    background:url(../assets/t11.jpg) no-repeat;
  }
  div.bg{
    position: absolute;
    width: 100%;
    height: 100%;
    background-size:cover;
    z-index: 3;
  }
  div.bg:target{ z-index: 9; }
  .a:target{ animation:a 1s; }
  @keyframes a{
    0% {transform:rotate(360deg) scale(0.1); }
    100%{transform:none;}
  }
  .b:target{ animation:b 1s;}
  @keyframes b{
    0% {transform: translateY(-1000px)}
    100%{transform: translateY(0)}
  }
  .c:target{ animation:c 1s; }
  @keyframes c{
    0% {transform:scale(0.1); }
    100%{transform:none; }
  }
  .d:target{ animation:d 1s; }
  @keyframes d{
    0% {transform:scale(2); }
    100%{transform:none;}
  }
  .e:target{ animation:e 1s; }
  @keyframes e{
    0% {transform: translate(1000px);}
    100%{transform: translate(0)}
  }
  .bg:not(:target){animation:ding 1s;}
  @keyframes ding{
    0% {z-index:3;}
    100%{z-index:3;}
  }

}
</style>
