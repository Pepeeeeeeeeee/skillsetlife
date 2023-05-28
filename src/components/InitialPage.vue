<template>
    <header>
        <nav class="navbar">
            <div class="nav-left">
                <a href="#"><img src="../assets/logo/Colorlogo-nobackground.svg" alt="" class="logo"></a>
                <div class = "comp divider">|</div>
                <div class = "comp"><a class="home-link" href="#">Your learning portal</a></div>
            </div>
            <div class="nav-right">
                <div class = "comp nm"><a href="#plans">PLÁNY</a></div>
                <div class = "comp nm"><a href="#faq">FAQ</a></div>
                <div class = "comp nm"><a href="#footer">KONTAKT</a></div>
                <div class = "comp divider">|</div>
                <div class = "comp social"><img src="../assets/instagram.svg"></div>
                <div class = "comp social"><img src="../assets/facebook.svg"></div>
            </div>
            <div class="nav-mobile" @click="toggleMobileNav()"><a id="navbar-toggle" href="#!"></a><span></span></div>
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
            <button class="cta-btn" @click ="move()" href>Začnite hneď </button>
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
        buy(){
            alert("Moving");
        },

        toggleMobileNav(){ 
            const hamburger = document.querySelector(".nav-mobile");
            hamburger.classList.toggle('active');
            
            const menu = document.querySelector('.nav-right');
            menu.classList.toggle('active')
        }
    },
    mounted() {
        document.querySelectorAll(".nm").forEach(n => n.addEventListener("click", this.toggleMobileNav));
    }
})
</script>

<style scoped>
    /* NAV */
    .navbar{
        background-color: #2395e2;
        display: flex;
        height: 56px;
        justify-content: space-between;
        z-index: 1;
        position: fixed;
        top: 0%;
        width: 100%;
    }
    .comp {
        padding: 0 16px;
        display: flex;
        align-items: center;
    }

    .comp  a {
        color: white;
    }
    .home-link {
        font-family: 'Times New Roman', Times, serif;
        font-size: large;
    }

    .divider {
        font-size: xx-large;
        color: white;
    }

    .nav-left {
        display: flex;
    }


    .nav-right {
        display: none;
        position: absolute;
        right: 0;
        top: 56px;
        text-align: right;
        padding: 16px;
        background-color:#2395e2;
        border-radius: 0 0 6px 6px;
    }
    
    .nav-right.active {
        display: block;
    }
    
    .nav-right .comp {
        text-align: right;
        justify-content: end;
        padding: 10px 16px;
        font-size: 1.4em;
    }

    .nav-right .divider, .nav-right .social {
        display: none;
    }

    .nav-mobile {
        display: flex;
        align-items: center;
        justify-content: center;      
    }

    #navbar-toggle {
     width: 45px;
     height: 45px;
    }

    .nav-mobile span, .nav-mobile span:before, .nav-mobile span:after {
     cursor: pointer;
     border-radius: 1px;
     height: 3px;
     width: 30px;
     background: #ffffff;
     position: absolute;
     display: block;
     content: '';
     transition: all 300ms ease-in-out;
    }

    .nav-mobile span:before {
        top: -10px;
    }
    .nav-mobile span:after {
        bottom: -10px;
    }
    .nav-mobile.active span {
        background-color: transparent;
    }
    .nav-mobile.active span:before, .nav-mobile.active span:after {
        top: 0;
    }
    .nav-mobile.active span:before {
        transform: rotate(45deg);
    }
    .nav-mobile.active span:after {
        transform: rotate(-45deg);
    }


    /* HERO */
    .bg {
        position: relative;
    }

    .bg img {
        width: 100%;
        height: 100%;
    }

    .bg-overlay {
        position:absolute;
        width: 100%;
        height:100%;
        top: 0%;
        left: 0%;
        background-color: rgba(42, 93, 165, 0.388);
    }

    .hero-container{
        display: grid;
    }

    .cont {
        position: absolute;
        place-self: center;
    }

    h1 {
        font-size: large;
        text-align: center;
        color: #ffffff;
    }

    .cta-btn{
        background-color: #2395e7;
        border: none;
        color: white;
        padding: 16px 24px;
        border-radius: 6px;
        font-size: large;
        width: fit-content;
        font-weight: bold;
        display: table;
        margin: 0 auto;
    }

@media screen and (min-width: 800px) {
    h1 {
        font-size: x-large;
        margin: 2em 0;
    }

    .cta-btn {
        font-size: x-large;
    }
    
}

@media screen and (min-width: 1000px) {
    .nav-right, .nav-right.active {
        display: flex;
        background: initial;
        position: initial;
    }

    .nav-mobile {
        display: none;
    }

    .nav-right .divider, .nav-right .social {
        display: flex;
        padding: .25em;
    }

    .nav-right .divider {
        font-size: xx-large;
        color: white;
    }
    
    .cont {
        place-self: center start;
        margin-left: 5%;
        width: 65%;
        max-width: 768px;
    }

    h1 {
        font-size: xx-large;
        text-align: left;
    }

    .cta-btn {
        margin: 10em auto 0 5%;
    }
}

    /* .btn2{
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
    } */
</style>