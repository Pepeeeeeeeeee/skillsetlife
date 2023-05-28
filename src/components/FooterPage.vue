<template>
    <footer id="footer">
        <div class = "footer">
            <div class="comp left">
                <img src = "../assets/logo/Colorlogo-nobackground.svg" class = "logo">
                <p class="divider">|</p>
                <div class = "contact">
                    <img src="../assets/contact-svgrepo-com.svg" class="icon">
                    <div>
                        <p>email@email.com <br> +421 948 569 954</p>
                    </div>
                </div>
            </div>
            <div class="comp middle">
                <a>copyright</a>
                <a>copyright1</a>
                <a>copyright2</a>
            </div>
            <div class="comp right">
                <img src="../assets/linkedin-svgrepo-com.svg" class = "icon">
                <img src="../assets/tiktok-svgrepo-com.svg" class = "icon">
                <img src="../assets/instagram.svg" class = "icon">
                <img src="../assets/facebook.svg" class = "icon">
            </div>
        </div>
    </footer>
</template>

<script>
export default ({
	name: "FooterPage",
	components: {
},
	data() {
		return {}
	},
    methods: {
    }
})
</script>

<style scoped>
    .icon {
        width: 50px;
        height: 50px;
    }
    .footer {
        background-color: #ABD2FF;
        display: grid;
        row-gap: 1em;
        padding: 1em;
        padding-bottom: 4px;
        margin-top: 2em;
    }

    .divider {
        display: none;
    }

    .comp.left {
        display: flex;
        justify-content: space-between;
    }

    .contact{
        display: grid;
        align-items: center;
        gap: 1em;
    }
    .contact .icon {
        grid-column: 2;
    }
    .contact div {
        grid-row: 1;
    }

    .comp.right {
        display: flex;
        grid-row: 2;
        place-self: center;
    }

    .comp.middle {
        place-self: center;
        display: flex;
        gap: 1em;
    }

@media screen and (min-width: 700px) {

    .footer{
        grid-template-columns: repeat(2, 1fr);
        row-gap: 0;
    }
    .divider {
        display: block;
        font-size: 3em;
        color: white;
        margin: 0;
    }

    .comp.left {
        display: flex;
        justify-content: start;
        align-items: center;
        gap: 1em;
    }

    .comp.right {
        place-self: center end;
        grid-column: 2;
        grid-row: 1;
    }

    .comp.middle {
        place-self: center end;
        transform: translateX(50%);
    }

    .contact .icon {
        grid-column: 1;
    }
    .contact div {
        grid-column: 2;
    }
}

@media screen and (min-width: 1280px) {
    .footer {
        grid-template-columns: repeat(3, 1fr);
    }

    .comp.middle{
        transform: initial;
        place-self: end center;
        grid-column: 2;
    }

    .comp.right {
        grid-column: 3;
    }
}

</style>