<template>
<div class="process-container">
  <h1>Ako to funguje?</h1>
  <div class="individuals">
    <h2>Pre jednotlivcov</h2> 
        <div class="sub-plans">
            <SubscriptionPage />
        </div>
    <div class="ind-process">
      <div class="step">
        <div class="step-img"><img src="../assets/credit-card.svg" alt=""></div>
        <h3>Vyber si</h3>
      </div>
      <img src="../assets/arrow-long-right.svg" alt="">
      <div class="step">
        <div class="step-img"><img src="../assets/key.svg" alt=""></div>
        <h3>Ziskaj pristup</h3>
      </div>
    </div>
  </div>

  <div class="organisations">
    <h2>Pre skoly/firmy:</h2>
    <div class="org-process">
      <div class="step">
        <div class="step-img"><img src="../assets/notes.svg" alt=""></div>
        <h3>Napiste nam</h3>
      </div>
      <img src="../assets/arrow-long-right.svg" alt="">
      <div class="step">
        <div class="step-img"><img src="../assets/sand-clock.svg" alt=""></div>
        <h3>Pockajte na odpoved</h3>
      </div>
      <img src="../assets/arrow-long-right.svg" alt="">
      <div class="step">
        <div class="step-img"><img src="../assets/key.svg" alt=""></div>
        <h3>Ziskajte pristup</h3>
      </div>
    </div>
    <h4><a href="#">Napiste nam</a> a spolocne prideme na prijatelnu cenu</h4>
    <!-- <button class = "button1">Napiste nam</button> -->
  </div>
</div>
</template>

<script>
import SubscriptionPage from './SubscriptionPage.vue';
export default ({
	name: "ProccesPage",
	components: {
    SubscriptionPage
},
	data() {
		return {}
	},
    methods: {
    }
})
</script>

<style scoped>
.process-container {
  width: 80%;
  margin: auto;
}

h1 {
  font-size: xx-large;
}

h2 {
  font-size: x-large;
  margin-left: 32px;
}

.individuals, .organisations{
  display: flex;
  flex-direction: column;
  position: relative;
  gap: 3em;
}

.sub-plans{
  margin: auto;
}

.ind-process, .org-process {
  display: flex;
  margin: auto;
  gap: 2em;
}
img {
  width: 56px;
}

.step {
  text-align: center;
  width: 182px;
}

h4 {
  font-size: x-large;
  text-align: center;
  margin-top: 0;
}

a {
  color: #2395E7;
}

.step-img{
  width: 64px;
  padding: 16px;
  margin: 10px auto;
  border-radius: 50%;
  background-color: #0047FF0D;
}

h3 {
  font-size: large;
}
  
</style>
