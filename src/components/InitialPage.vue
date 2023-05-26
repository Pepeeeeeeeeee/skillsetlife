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
    <div class = "hero-container">
        
        <div class="bg">
            <img src="../assets/pexels-alena-darmel-9040431.jpg" class="bg-img">
            <div class="bg-overlay"></div>
        </div>

            <div class = "cont">
                <h1>“Dosiahni svoje ciele s naším skvelým vzdelávacím nástrojom ”</h1>
                <button class="btn2" @click ="move()">Zacnite hned</button>
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
      .btn2{
        background-color: #2395e7;
        border: none;
        color: white;
        padding: 16px 24px;
        border-radius: 6px;
        font-size: xx-large;
        width: fit-content;
        font-weight: bold;
    }

    .bg {
        position: relative;
    }

    .bg > img {
        width: 100%;
    }

    .bg-overlay {
        position:absolute;
        width: 100%;
        height:100%;
        top: 0%;
        left: 0%;
        background-color: rgba(42, 93, 165, 0.388);
    }

    .cont {
        position: absolute;
        display: flex;
        flex-direction: column;
        gap: 12em;
        font-size: large;
        color: white;
        top: 25%;
        left: 12em;
    }

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
 
    .logo{
        height: 56px;
    }
</style>