<template>
  <div class= "hero">
    <div class="content">
      <h1 id="title">
        <slot name = "heroh1"></slot>
      </h1>
      <p id="description">
        <slot name = "description"></slot>
      </p>
      <ActionButton>Read More</ActionButton>
    </div>
  </div>
</template>
<style scoped>
.hero{
  background-image:url("../assets/images/herosectionbg.jpg");
 background-repeat: no-repeat;
 background-size:100% 100%;
 width: 80%;
 height: 90vh;
 margin: 0 auto;
}
.content{
  margin-left:10%;
  padding-top:10%;
}
#title{
  color: antiquewhite;
  font-size: 6.5vh;
  font-family:'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
}
#description{
  color: rgb(197, 82, 5);
  font-size: 2vh;
  width: 35%;
}
</style>