<template>
    <div class = "bgr">
        <div>
            <h3 class = "text" @click="help()">Pomoze s dosahovanim uspechu, ochrani pred <br> dezinformaciami a manipulaciami, pomoze so <br> zarobenim penazi</h3>
        </div>
        <div class = "compo">
            <div class="icon-bg">
                <img src="../assets/list.svg" alt="" class = "icon">
            </div>
            <div class="">
                <p>Ucebne Formaty</p>
                <ul>
                    <li>Kurzy</li>
                    <li>Podcasty</li>
                    <li>Shorty</li>
                    <li>Pitch nights</li>
                    <li>Cvicenia</li>
                </ul>
            </div>
        </div>
        <div class = "compo">
            <div class="icon-bg">
                <img src="../assets/calendar.svg" alt="" class = "icon">
            </div>
            <div class="">
                <p>Komunitne podujatias</p>
                <ul>
                    <li>Diskusie</li>
                    <li>Livestreamy</li>
                    <li>Eventy</li>
                </ul>
            </div>
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
        margin-bottom: 2em;
        display: flex;
        flex-direction: row;
        justify-content:center;
        gap: 12em;
    }

    .text{
        font-weight: bolder;
        font-size: x-large;
        line-height: 2em;
    }

    .compo {
        display: flex;
        gap: 1em;
    }
    

    .icon-bg {
        height: 48px;
        width: 48px;
        padding: 16px;
        border-radius: 100%;
        background-color: #44a5eb;
    }

    .icon{
        width: 48px;
    }

    li {
        font-size: large;
    }

    p {
        font-size: larger;
        font-weight: bold;
    }

</style>