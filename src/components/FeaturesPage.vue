<template>
    <h1 class="title">Výhody a vlastnosti</h1>
    <div class = "features-container">
        <div class="cont">
            <div class="col top">
                <h3 class = "text-title">Pomôže s dosahovaním úspechu, ochráni pred <br> dezinformáciami a manipuláciami, pomôže so <br> zarobením peňazí</h3>
                <h4 class = "text">Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.
                        Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. 
                        Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. 
                        Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.</h4>
            <button class="cta-btn" @click="buy()">KÚPIŤ</button>
            </div>
            <div class="col bot">
                <div class = "compo">
                    <div class="formats">
                        <div class="icon-bg"><img src="../assets/list.svg" alt="" class = "icon"></div>
                        <div class="">
                            <p>Učebne Formáty</p>
                            <ul>
                                <li>Kurzy</li>
                                <li>Podcasty</li>
                                <li>Shorty</li>
                                <li>Pitch nights</li>
                                <li>Cvičenia</li>
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
                            <p>Komunitné podujatia</p>
                            <ul>
                                <li>Diskusie</li>
                                <li>Live streamy</li>
                                <li>Eventy</li>
                            </ul>

                        </div>
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
        buy(){
            alert("Moving");
        },
    }
})
</script>
<style scoped>
.features-container{
    background-color: #2395E7;
    color: white;
    margin-bottom: 2em;
}

.cont {
    max-width: 1600px;
    margin: 0 auto;
    display: grid;
    padding: 2em;
}

.col.bot {
    display: flex;
    justify-content: space-around;
}

h4 {
    font-weight: 100;
}

.formats, .events {
    display: flex;
    flex-direction: column;
    align-items: center;
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

.stock {
    display: none;
}

.cta-btn {
        padding: .5em 1.5em;
        font-size: large;
        background-color: #2395E7;
        border: 2px white solid;
        color: white;
        text-align: center;
        border-radius: 6px;
        display: table;
        margin: 2em auto;
    }

@media screen and (min-width: 800px) {
    .cont{
        gap: 2.5em;
    }
    .col.bot {
        grid-column: 2;
        place-self: center;
        gap: 1em;
    }

}

@media screen and (min-width: 1280px) {

    .stock{
        width: 300px;
        height: 200px;
        border-radius: 12px;
        display: block;
    }

    .col.top {
        place-self: center;
    }

    .col.bot {
        display: block;
    }

    .compo {
        display: flex;
        flex-direction: row;
        align-items: center;
        gap: 1em;
        margin: 1em 0 3em;
    }

    .formats, .events{
        width: 280px;
    }

    .text-title{
        font-weight: bolder;
        font-size: x-large;
        line-height: 1em;
    }

    .text{
        font-size: x-large;
        font-weight: lighter;
        max-width: 700px;
    }

    li {
        font-size: large;
    }
    p {
        font-size: larger;
        font-weight: bold;
    }
    .cta-btn {
        font-size: xx-large;
    }
    
}
</style>