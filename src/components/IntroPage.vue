<template>
    <div class = "bgr">
        <div class="col">
            <h3 class = "textNadpis" @click="help()">Pomoze s dosahovanim uspechu, ochrani pred <br> dezinformaciami a manipulaciami, pomoze so <br> zarobenim penazi</h3>
            <div>
                <h4 class = "text">Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.
                     Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. 
                     Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. 
                     Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.</h4>
            </div>
        <button>KUPIT</button>
        </div>
        <div class="col">
            <div class = "compo">
                <div class="formats">
                    <div class="icon-bg"><img src="../assets/list.svg" alt="" class = "icon"></div>
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
                <img src ="../assets/courseimg.jpg" class = "stock">
            </div>
            <div class = "compo">
                <img src ="../assets/eventimg.jpg" class = "stock">
                <div class="events">
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
<style scoped>

.formats, .events {
    width: 280px;
    display: flex;
    flex-direction: column;
    align-items: center;
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
        padding: 2em;
    }

    .col {
        display: flex;
        flex-direction: column;
        justify-content: center;
        gap: 2em;
    }

    button {
        width:128px;
        height: 64px;
        align-self: center;
        font-size: xx-large;
        background-color: #2395E7;
        border: 2px white solid;
        color: white;
        text-align: center;
        border-radius: 6px;
    }

    .stock{
        width: 300px;
        height: 200px;
        border-radius: 12px;
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
        flex-direction: row;
        align-items: center;
        gap: 1em;
        margin: 1em 0 3em;
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
    img {
        display: flex;
    }

</style>