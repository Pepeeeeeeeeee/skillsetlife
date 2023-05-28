<template>
        <h1 class="title" id="plans">Lorem ipsum dolor sit.</h1>
        <h3 class="subtitle">Lorem, ipsum dolor.</h3>
    <div class = "subscriptions-container">
        <div class = "card monthly">
            <p class="header">/</p>
            <h4>Mesacny</h4>
            <h2>12.99$</h2>
            <h5>mesacne</h5>
            <div class="step">
                <div class="step-img"><img src="../assets/credit-card.svg" alt=""></div>
                <h3>Ziskajte okamzity pristup k obsahu</h3>
            </div>
            <h6>* iba pre jednotlivcov</h6>
            <button @click = "pay()" class = "btn">Pokraovat</button>
        </div>
        <div class = "card yearly">
            <p class="header">Usetrite XX%</p>
            <h4>Rocny</h4>
            <h2>129$</h2>
            <h5>rocne</h5>
            <div class="step">
                <div class="step-img"><img src="../assets/credit-card.svg" alt=""></div>
                <h3>Ziskajte okamzity pristup k obsahu</h3>
            </div>
            <h6>* iba pre jednotlivcov</h6>
            <button @click = "pay()" class = "btn">Pokraovat</button>
        </div>
        <div class = "card orgs">
            <p class="header">Pre Firmy a Skoly</p>
            <div class="org-process">
                <div class="step">
                    <div class="step-img"><img src="../assets/notes.svg" alt=""></div>
                    <h3>Napiste nam</h3>
                </div>
                <div class="step">
                    <div class="step-img"><img src="../assets/pen.svg" alt=""></div>
                    <h3>Dohodneme sa na podmienkach</h3>
                </div>
            </div>

            <button @click = "pay()" class = "btn">Pokraovat</button>
        </div>

        <Form id = "overlay" />
        
    </div>
</template>
<script>
import Form from './FormPage.vue';
export default ({
	name: "SubscriptionPage",
	components: {
        Form,
	},
	data() {
		return {
            visible: false,
        }
	},
    methods: {
        pay(){
            if(this.visible == false){
                document.getElementById("overlay").style.visibility = "visible";
                this.visible = true;
            }

            else if(this.visible == true){
                document.getElementById("overlay").style.visibility = "hidden";
                this.visible = false;
            }
        }
    }
})
</script>
<style scoped>
#overlay{
    visibility: hidden;
    position: absolute;
}

    .subtitle {
        text-align: center;
    }

    .card{
        margin: 1em auto;
        width: 188px;
        height: 232px;
        border: 2px solid black;
        text-align: center;
        border-radius: 16px;
    }

    h2, h3, h5 {
        margin: 0;
    }

    h3 {
        font-size: small;
    }

    h4 {
        margin: .25em 0;
    }

    h5 {
        font-weight: 500;
        font-style: italic;
    }

    h6 {
        margin: 1em 0;
    }

    .step {
        margin: .5em 0;
    }
    
    .btn{
        width: 90%;
        background-color: #2395e7;
        border: none;
        color: white;
        padding: 4px;
        border-radius: 6px;
    }

    .card:hover{
        border-color: #2395E7;
        color: #2395E7;
    }

    .header {
        box-sizing: border-box;
        border-radius: 14px 14px 0 0 ;
        margin: 0;
        padding: 6px;
        color: white;
    }

    .yearly > .header {
        background-color: #2395E7;
    }

    .orgs > .header {
        margin: 12px 0 24px;
        color: black;
    }

@media screen and (min-width: 800px) {
    .subscriptions-container {
        display: flex;
        justify-content: space-evenly;
        max-width: 1000px;
        margin: 0 auto;
    }
}

@media screen and (min-width: 1000px) {
    .card{
        width: 224px;
        height: 304px;
    }

    h2 {
        font-size: xx-large;
    }

    h3 {
        margin: 8px 16px;
    }

    h4 {
        margin: 1em 0 4px 0;
        font-size: larger;
    }

    h6 {
        margin: 0 4px 12px;
    }

    .step {
        margin-bottom: 1.4em;
    }
}
/*
    .subscriptions-container{
	display: flex;
    gap: 5em;
    justify-content: center;
    }

    .card{
        width: 224px;
        height: 304px;
        border: 2px solid black;
        text-align: center;
        border-radius: 16px;
    }
    
    .btn{
        width: 90%;
        background-color: #2395e7;
        border: none;
        color: white;
        padding: 4px;
        border-radius: 6px;
    }

    h2 {
        font-size: xx-large;
        margin: 0;
    }
    h5 {
        margin-top: 0;
        font-weight: 500;
        font-style: italic;

    }
    h3 {
        margin: 8px 16px;
        font-size: small;

    }

    h4 {
        margin: 1em 0 4px 0;
        font-size: larger;
    }

    h6 {
        margin: 0 4px 12px;
    }

    .card:hover{
        border-color: #2395E7;
        color: #2395E7;
    }

    .header {
        box-sizing: border-box;
        border-radius: 14px 14px 0 0 ;
        margin: 0;
        padding: 6px;
        color: white;
    }

    .yearly > .header {
        background-color: #2395E7;
    }

    .orgs > .header {
        margin: 12px 0 24px;
        color: black;
    }

    .step {
        margin-bottom: 1.4em;
    }

    .org-process {
        display: flex;
        flex-direction: column;
        gap: 16px;
    } */

    
</style>