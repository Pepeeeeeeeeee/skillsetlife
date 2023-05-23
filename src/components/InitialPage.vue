<template>
    <header>
        <div class="container">
            <!-- <div class = "logo"><img src="../assets/ColorLogoWithBG.svg"></div> -->
            <div class = "comp"><a>AKO TO FUNGUJE?</a></div>
            <div class = "comp"><a>FAQ</a></div>
            <div class = "comp"><a>KONTAKT</a></div>
            <div class = "comp">|</div>
            <div class = "comp"><img src="../assets/instagram.png"></div>
            <div class = "comp"><img src="../assets/facebook.png"></div>
        </div>
        <title>skillset.life</title>
    </header>
    <div class = "bg">


            <div class = "cont">
                <h1>“Dosiahni svoje ciele s naším skvelým vzdelávacím nástrojom”</h1>
                <button @click ="move()">Zacnite hned</button>
            </div>

            <!-- <table>
                <tr>
                    <th><h4>Kontakt :</h4></th>
                    <th><h4>email@email.com</h4></th> 
                    <th><h4>+421956 809 876</h4></th>   
                </tr>
            </table> -->
    </div>
</template>

<script>
export default ({
	name: "ProccesPage",
	components: {
},
	data() {
		return {}
	},
    methods: {
        move(){
            alert("Moving");
        }
    }
})
</script>

<style>

    
    .container{
        display: flex;
        flex-direction: row;    
        float: right;
    }
    
    .comp{
        padding-left: 20px;
    }

    .cont{
        padding-top: 100px;
    }

    .bg{
	background-image: url(../assets/background.svg) !important;
	background-repeat: no-repeat;
	background-attachment: fixed;
	background-size: 100% 100%;
    }
 
    .logo{
        width: 16px;
        height: 16px;
    }
</style>