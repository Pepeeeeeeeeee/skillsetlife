<template>
    <footer>
        <div class = "footer">
            <div>
                <img src = "../assets/logo/Colorlogo-nobackground.svg" class = "logo">
            </div>
            <div>
                |
            </div>
            <div class = "contact">
                <div>
                    <img src="../assets/contact-svgrepo-com.svg">
                </div>
                <div>
                    <p>email@email.com <br> +421 948 569 954</p>
                </div>
            </div>
            <div>
                <a>copyright</a>
            </div>
            <div>
                <a>copyright1</a>
            </div>
            <div>
                <a>copyright2</a>
            </div>
            <div>
                <img src="../assets/linkedin-svgrepo-com.svg" class = "iconFooter">
            </div>
            <div>
                <img src="../assets/tiktok-svgrepo-com.svg" class = "iconFooter">
            </div>
            <div>
                <img src="../assets/instagram.svg" class = "iconFooter">
            </div>
            <div>
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

<style>
    .footer{
        margin-top: 50px;
        display: flex;
        flex-direction: row;
        background-color: #ABD2FF;
    }

    .iconFooter{
        width: 50px;
        height: 50px;
    }

    .contact{
        display: flex;
        flex-direction: row;
    }
</style>