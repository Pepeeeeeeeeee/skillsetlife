<template>
   <h3>Partneri</h3>
        <div id="logos"> 
            <div id="logosPrev">
                <img id="logo" src="../assets/bk.png" >
                <img id="logo" src="../assets/MSVVAS.png" >
                <img id="logo" src="../assets/spsehalova.png" >
                <img id="logo" src="../assets/400square-legacy.jpg" >
            </div>
            <div id="logosNext">
                <img id="logo" src="../assets/400square-legacy.jpg" >
                <img id="logo" src="../assets/400square-legacy.jpg" >
                <img id="logo" src="../assets/400square-legacy.jpg" >
                <img id="logo" src="../assets/400square-legacy.jpg" >
            </div>
        </div>
    <h3>Benefits & Features</h3>
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
    #logo
{
    width: auto;
    max-height: 130px;
    margin: 3%;
    /*border: dotted black 2px;*/ 
}

#logos
{
    border-bottom: solid black 2px;
    width: 70%;
    text-align: center;
    margin-left: auto;
    margin-right: auto;
    margin-top: 4%;
    margin-bottom: 4%;
}

#logoToggle
{
    display:inline;
    float:left;
}
</style>