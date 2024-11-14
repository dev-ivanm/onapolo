<template>
  <section>
    <img src="../../assets/img/1.jpg" alt="" />
    <img src="../../assets/img/2.jpg" alt="" />
    <img src="../../assets/img/4.jpg" alt="" />
    <img src="../../assets/img/3.jpg" alt="" />
    <img src="../../assets/img/5.jpg" alt="" />
    <img src="../../assets/img/6.jpg" alt="" />
  </section>
</template>

<script></script>
<style scope>
section {
  display: flex;
  width: 600px;
  height: 430px;  
}

section img{
  width: 0px;
  flex-grow: 1;
  object-fit: cover;
  opacity: .8;
  transition: .5s ease;
}

section img:hover{
  cursor: crosshair;
  width: 300px;
  opacity: 1;
  filter: contrast(120%);
}
</style>
