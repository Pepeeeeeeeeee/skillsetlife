<template>
    <h1 class="title" id="faq">Často kladené otázky</h1>
    <div class="faq-container">

        <div class="questions">
            <div class="question left" @click="toggleShow(1)">
                <h3>Lorem ipsum dolor sit amet</h3>
                <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.
                    Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.
                    Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
                    Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.
                </p>
            </div>

            <div class="question right" @click="toggleShow(2)">
                <h3>Lorem ipsum dolor sit amet</h3>
                <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.
                    Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.
                    Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
                    Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.
                </p>
            </div>

            <div class="question left" @click="toggleShow(3)">
                <h3>Lorem ipsum dolor sit amet</h3>
                <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.
                    Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.
                    Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
                    Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.
                </p>
            </div>

            <div class="question right" @click="toggleShow(4)">
                <h3>Lorem ipsum dolor sit amet</h3>
                <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.
                    Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.
                    Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
                    Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.
                </p>
            </div>

            <div class="question left" @click="toggleShow(5)">
                <h3>Lorem ipsum dolor sit amet</h3>
                <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.
                    Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.
                    Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
                    Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.
                </p>
            </div>
        </div>
    </div>
</template>

<script>
export default ({
	name: "FooterPage",
	components: {
},
	data() {
		return {
        }
	},
    methods: {
        toggleShow(i){
            var x = document.getElementsByClassName('question')[i-1];
            x.classList.toggle('active');
        }
    }
})
</script>

<style scoped>
    .active p {
        display: block;
    }

    .left h3:after{
        margin-left: 1em;
        content: '⮟';
    }

    .active.left h3:after {
        margin-left: 1em;
        content: '⮝';
    }
    .right h3:before{
        margin-right: 1em;
        content: '⮟';
    }

    .active.right h3:before {
        margin-right: 1em;
        content: '⮝';
    }

    h3 {
    padding: .6em;
    text-align: center;
    font-size: 16px;
    background-color: #2395e7;
    color: white;
    }

    p {
        max-width: 615px;
        width: 90%;
        font-size: 14px;
        margin: 0 1.5em;
        display: none;
    }

@media screen and (min-width: 800px) {
    p {
        font-size: 16px;
    }

    .question {
        margin-bottom: 3em;
    }

    .question.left {
        margin-right: 25%;
    }
   .question.left h3 {
        text-align: right;
        padding-right: 2.5em;
        border-radius: 0 8px 8px 0;
    }
    .question.left p {
        margin-left: auto;
    }
    .question.right {
        margin-left: 25%;
    }
    .question.right h3 {
        text-align: left;
        padding-left: 2.5em;
        border-radius: 8px 0 0 8px;
    }
}

@media screen and (min-width: 1280px) {
    .question.left {
        margin-right: 40%;
    }
    .question.right {
        margin-left: 40%;
    }
}
</style>