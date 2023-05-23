<template>
    <div class = "subscriptions-container">
        <div class = "card monthly">
            <p class="sale">/</p>
            <h4>Mesacny</h4>
            <h2>12.99$</h2>
            <h5>mesacne</h5>
            <button @click = "pay()" class = "button1">Pokraovat</button>
        </div>
        <div class = "card yearly">
            <p class="sale">Usetrite XX%</p>
            <h4>Rocny</h4>
            <h2>129$</h2>
            <h5>rocne</h5>
            <button @click = "pay()" class = "button1">Pokraovat</button>
        </div>
    </div>
</template>
<script>
export default ({
	name: "SubscriptionPage",
	components: {
	},
	data() {
		return {}
	},
    methods: {
        pay(){
            alert("Works")
        }
    }
})
</script>
<style>
    .subscriptions-container{
	display: flex;
	flex-direction: row;
    gap: 5em;
    }

    .card{
        width: 196px;
        height: 220px;
        border: 2px solid black;
        text-align: center;
        border-radius: 16px;
    }
    
    .button1{
        width: 90%;
    }

    h2 {
        font-size: xx-large;
        margin-bottom: 0;
    }
    h5 {
        margin-top: 0;
        font-weight: 500;
        font-style: italic;

    }

    .card:hover{
        border-color: #2395E7;
        color: #2395E7;
    }

    .sale {
        box-sizing: border-box;
        border-radius: 14px 14px 0 0 ;
        margin: 0;
        padding: 6px;
        color: white;
    }

    .yearly > .sale {
        background-color: #2395E7;
    }
</style>