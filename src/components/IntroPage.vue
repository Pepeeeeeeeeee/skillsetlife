<template>
    <div class = "bgr">
        <div>
            <h3 class = "text" @click="help()">Pomoze s dosahovanim uspechu, ochrani pred <br> dezinformaciami a manipulaciami, pomoze so <br> zarobenim penazi</h3>
        </div>
        <div class = "compo">
            <img src="../assets/mortarboard.png" alt="" class = "icon">
            <p>
                Kurzy <br><br>
                Podcasty <br><br>
                Shorty <br><br>
                Pitch nights <br><br>
                Cvicenia
            </p>
        </div>
        <div class = "compo">
            <img src="../assets/event.png" alt="" class = "icon">
            <p>
                Diskusie <br><br>
                Livestreamy <br><br>
                Eventy
            </p>
        </div>
    </div>
</template>
<script>
export default ({
	components: {
	},
	data() {
		return {}
	},
    methods: {
        help(){
            alert("Help")
        }
    }
})
</script>
<style>
    .bgr{
        background-color: #2395E7;
        padding: 2em;
        color: white;
        padding-bottom: 2em;
        margin-bottom: 2em;
        display: flex;
        flex-direction: row;
    }

    .text{
        font-weight: bolder;
        font-size: x-large;
        line-height: 2em;
    }
 
    .compo{
        
        margin-left: 100px;

    }

    .icon{
        size: 64px;
        border: solid;
        border-radius: 100%;
    }
</style>