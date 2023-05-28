<template>
    <h1 class="title">Partneri</h1>
    <div class="partners-container">
        <div class="logos"> 
            <img class="logo" src="../assets/bk.png" >
            <img class="logo" src="../assets/MSVVAS.png" >
            <img class="logo" src="../assets/spsehalova.png" >
            <img class="logo" src="../assets/400square-legacy.jpg" >
            <img class="logo" src="../assets/400square-legacy.jpg" >
            <img class="logo" src="../assets/400square-legacy.jpg" >
            <img class="logo" src="../assets/400square-legacy.jpg" >
            <img class="logo" src="../assets/400square-legacy.jpg" >
        </div>
    </div>
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
.logo {
    width: auto;
    max-height: 130px;
    margin: 3%;
}

.logos {
    border-bottom: solclass black 2px;
    width: 80%;
    text-align: center;
    margin: 0 auto;
}
</style>