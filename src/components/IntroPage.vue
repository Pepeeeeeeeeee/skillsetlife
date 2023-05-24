<template>
    <div class = "bgr">
        <div>
            <h3 class = "textNadpis" @click="help()">Pomoze s dosahovanim uspechu, ochrani pred <br> dezinformaciami a manipulaciami, pomoze so <br> zarobenim penazi</h3>
            <div>
                <h4 class = "text">Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.
                     Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. 
                     Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. 
                     Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.</h4>
            </div>
            <div><button>KUPIT</button></div>
        </div>
        <div class = "compo">
            <div class = "compo1">
                <div class = "compo1_1">
                    <div class="icon-bg">
                        <img src="../assets/list.svg" alt="" class = "icon">
                    </div>
                    <div><img src ="../assets/courseimg.jpg" class = "stock"></div>
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
        </div>
        <div class = "compo">
            <div class = "compo2">
                <div class = "compo2_2">
                    <div class="icon-bg">
                        <img src="../assets/calendar.svg" alt="" class = "icon">
                    </div>
                    <div><img src ="../assets/eventimg.jpg" class = "stock"></div>
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
    .compo2{
        margin-top: 400px;
    }

    .compo1_1{
        display: flex;
        flex-direction: row;
    }

    .compo2_2{
        display: flex;
        flex-direction: row;
    }

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

    .stock{
        width: 300px;
        height: 200px;
        margin-left: 12em;
    }

    .textNadpis{
        font-weight: bolder;
        font-size: x-large;
        line-height: 1em;
    }

    .text{
        padding-top: 10px;
        padding-left: 15px;
        font-weight: lighter;
        width: 700px;
    }

    .compo {
        display: flex;
        flex-direction: column;
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