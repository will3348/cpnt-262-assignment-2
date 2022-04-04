<template>
  <div class="card">
    <div class="card-image">
      <img :src="card.image"/>
    </div>
    <div class="card-title">
      {{card.title}}
    </div>
    <div class="card-text">
      {{card.text}}
    </div>
    <div class="card-CTA">
      <button>Learn More</button>
    </div>
    
  </div>
</template>
<script>
export default {name: 'TheCard',
  props: {
  card: {
      type: Object,
      required: true,
  	},
  }
}

</script>

<style scoped>
 .card{
   border: 1px solid rgb(255, 255, 255);
   width: 400px;
   height: 500px;
   margin-top:30px;
   position: relative;
 }
 img{
   width: 100%;
   height: 250px;
 }
 .card-title{
   font-size: 4vh;
   font-weight: bolder;
 }
 .card-text{
   margin: 15px;
 }
 button{
   position: fixed;
  color: forestgreen;
  background-color: transparent;
  border: red 1px solid;
  border-radius: 5px;
  width: 200px;
  height: 30px;
  position: absolute;
  bottom: 0;
  left: 20%;
 }
</style>
