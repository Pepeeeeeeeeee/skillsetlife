<template>
    <header>
        <nav class="navbar">
            <div class="nav-left">
                <img src="../assets/logo/Colorlogo-nobackground.svg" alt="" class="logo">
                <div class = "comp divider">|</div>
                <div class = "comp"><a class="home-link">Your learning portal</a></div>
            </div>
            <div class="nav-right">
                <div class = "comp"><a>PREDPLATNE</a></div>
                <div class = "comp"><a>FAQ</a></div>
                <div class = "comp"><a>KONTAKT</a></div>
                <div class = "comp divider">|</div>
                <div class = "comp social"><img src="../assets/instagram.svg"></div>
                <div class = "comp social"><img src="../assets/facebook.svg"></div>
            </div>
        </nav>
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
    .home-link {
        font-family: 'Times New Roman', Times, serif;
        font-size: x-large;
    }

    .navbar{
        display: flex;
        height: 56px;
        justify-content: space-between;
        z-index: 1;
        position: fixed;
        top: 0%;
        width: 100%;
    }

    .nav-left, .nav-right {
        display: flex;
    }
    
    .comp {
        padding: 0 16px;
        display: flex;
        align-items: center;
    }

    .divider {
        font-size: xx-large;
    }

    .cont{
        padding-top: 100px;
    }

    /* .bg{
	//background-image: url(../assets/background.svg) !important;
	background-repeat: no-repeat;
	background-attachment: fixed;
	background-size: 100% 100%;
    } */
 
    .logo{
        height: 56px;
    }
</style>