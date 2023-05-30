<template>
    <h1 class="title" id="faq">FAQ</h1>
    <div class="faq-container">

        <div class="questions">
            <div class="question left" @click="show(1)">
                <h3 id = "que1">Lorem ipsum dolor sit amet</h3>
                <p id = "ans1">Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.
                    Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.
                    Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
                    Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.
                </p>
            </div>

            <div class="question right" @click="show(2)">
                <h3 id = "que2">Lorem ipsum dolor sit amet</h3>
                <p id = "ans2">Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.
                    Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.
                    Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
                    Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.
                </p>
            </div>

            <div class="question left" @click="show(3)">
                <h3 id = "que3">Lorem ipsum dolor sit amet</h3>
                <p id = "ans3">Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.
                    Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.
                    Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
                    Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.
                </p>
            </div>

            <div class="question right" @click="show(4)">
                <h3 id = "que4">Lorem ipsum dolor sit amet</h3>
                <p id = "ans4">Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.
                    Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat.
                    Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur.
                    Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.
                </p>
            </div>

            <div class="question left" @click="show(5)">
                <h3 id = "que5">Lorem ipsum dolor sit amet</h3>
                <p id = "ans5">Lorem ipsum dolor sit amet, consectetur adipiscing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua.
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
        show(i){
            document.getElementById("ans" + [i]).style.visibility = "visible";
        }
    }
})
</script>

<style scoped>
    #ans1{
        visibility: hidden;
    }
    #ans2{
        visibility: hidden;
    }
    #ans3{
        visibility: hidden;
    }
    #ans4{
        visibility: hidden;
    }
    #ans5{
        visibility: hidden;
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