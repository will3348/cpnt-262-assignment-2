<template>
<div>
  <div class="herosection" >
    <TheHero>
      <template v-slot:heroh1>
       You Dream It!<br />We Build It!
      </template>
      <template v-slot:description >
        A symbol of style and a bespoke creator of vehicles of purity, elegance
        and innovation. We focus on design, engineering, conception and
        production of bespoke vehicles for discerning clientele that require
        more.
      </template>
      <template v-slot:CTA id="cta">Read More </template>
    </TheHero>
  </div>
  <div class="card-section">
   <TheCard v-for="card in cards" :key="card.id"
  :card="card">
    </TheCard>
  </div>
 </div> 
</template>
<script>
import TheCard from './TheCard.vue'
const cards = [
  {
    title: "Engine" , 
    text:"Engine tuning is the adjustment or modification of the internal combustion engine or Engine Control Unit (ECU) to yield optimal performance and increase the engine's power output, economy, or durability" ,
    tags:["rachet","2people","sport"],
    image:('../assets/images/engineimage.png'),
    id:1
  },

  {
    title: "Exhaust" , 
    text:"An automotive exhaust system is a fantastic piece of engineering. Its primary purpose is to remove exhaust gases from a combustion engine while reducing the noise produced by the entire process." ,
    tags:["rachet","2people","sport"],
    image:('../assets/images/exhaust.webp'),
    id:2

  },

  {
    title: "Suspension" , 
    text:"Ample clearance height, better handling, easier towing and the opportunity to fit tyres with bigger tread than the stock market tyres your vehicle was fitted with at the factory" ,
    image:('../assets/images/suspension.webp'),
    id:3

  },


]
export default {
  components: {
    TheCard
  },
  data(){
    return {cards}
  }
}
</script>
<style scoped>
.card-section{
  margin:0 auto;
  width:70%;
  display: flex;
  justify-content:space-around ;
}
</style>