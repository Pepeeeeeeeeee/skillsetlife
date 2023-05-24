<template>
    <footer>
        <div class = "footer">
            <div class="comp left">
                <img src = "../assets/logo/Colorlogo-nobackground.svg" class = "logo">
                <p class="divider">|</p>
                <div class = "contact">
                    <img src="../assets/contact-svgrepo-com.svg" class="iconFooter">
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
                <img src="../assets/linkedin-svgrepo-com.svg" class = "iconFooter">
                <img src="../assets/tiktok-svgrepo-com.svg" class = "iconFooter">
                <img src="../assets/instagram.svg" class = "iconFooter">
                <img src="../assets/facebook.svg" class = "iconFooter">
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
    .footer{
        margin-top: 50px;
        width: 100%;
        height: 64px;
        display: flex;
        flex-direction: row;
        background-color: #ABD2FF;
        justify-content: space-between;
        color: white;
    }

    .comp {
        width: 33%;
        gap: 1em;

    }

    .right {
        justify-content: right;
    }

    .left {
        justify-content: left;
    }

    .middle {
        justify-content: center;
    }
    

    .iconFooter{
        width: 50px;
        height: 50px;
    }

    .contact{
        display: flex;
        align-items: center;
        gap: 1em;
    }

</style>