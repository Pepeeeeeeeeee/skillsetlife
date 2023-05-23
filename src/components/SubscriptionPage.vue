<template>
    <div class = "subscriptions-container">
        <div class = "card">
            <h4 class = "h4">Mesacny</h4>
            <h2>12.99$</h2>
            <h5>mesacne</h5>
            <button @click = "pay()" class = "button1">Pokraovat</button>
        </div>
        <div class = "card">
            <h4 class = "h4">Rocny</h4>
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
    }

    .card{
        margin-right: 100px;
        width: 15%;
        height: 200px;
        border-style: solid;
        border-color: black;
    }
    
    .button1{
        width: 90%;
    }

    .h4{
        padding-top: 5%;
    }
</style>