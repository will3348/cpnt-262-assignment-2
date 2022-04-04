<template>
  <div>
    <ul class="navi-bar">
      <li>
        <a href="/">Home</a>
      </li>
      <li>
        <a href="/">Service</a>
      </li>
      <li>
        <a href="/">About us</a>
      </li>
      <li>
        <a href="/">Contact</a>
      </li>
    </ul>
  </div>
</template>
<style scoped>
.navi-bar{
  display: flex;
  flex-direction: row;
  gap: 30px;
  margin-top: 25px;
  padding: 0px;
}
li{
  width: 90px;
  text-align: center;
}
li:hover{
  background-color: blue;
  color: antiquewhite;
  border-radius: 15px;
}
</style>
