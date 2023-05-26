<template>
    <div class = "formbg">
        <form action = "../php/register.php" method = "post">
            
            <h2 style = "margin-bottom: -1rem;">Zadajte udaje</h2>
            <h3>Ozveme sa vam hned ako to bude mozne</h3>
            
            <div class = "form_group">
                <i class = "gg-profile" style = "top: 19px; scale: 185%"></i>
                <input name = "full_name" type = "text" class = "form_align" placeholder = "Zadajte vase cele meno...">
            </div>
            
            <div class = "form_group">
                <i class="gg-mail" style = "top: 22px; scale: 180%"></i>
                <input name = "mail" type = "email" class = "form_align" placeholder = "Zadajte vas email...">
            </div>
    
            <div class = "form_group">
                <i class="gg-phone" style = "top: 20px; scale: 150%"></i>
                <input name = "phone_number" type = "text" class = "form_align" placeholder = "Zadajte vase cislo...">
            </div>
    
            <div class = "form_group">
                    <i class="gg-organisation" style = "top: 19px"></i>
                    <select name = "organization" class = "form_align" onchange = "Osaker()">
                        <option value = "" disabled selected hidden>Zadajte typ organizacie...</option>
                        <option value = "Skola">Skola</option>
                        <option value = "Firma">Firma</option>
                        <option value = "Statna institucia">Statna institucia</option>
                        <option value = "Ine" id = "opt">Ine</option>
                    </select>
            </div>
    
            <div style = "display: none;" class = "form_group" id = "checked">
                <input name = "other" type = "text" class = "form_align" id = "txt" placeholder = "Typ organizacie...">
            </div>
    
            <div class = "form_group">
                    <i class="gg-user" style = "left: 30px; scale: 180%"></i>
                    <select name = "amount" class = "form_align">
                        <option value = "" disabled selected hidden>Zadajte pocet ludi...</option>
                        <option value = "1-10">1-10</option>
                        <option value = "10-100">10-100</option>
                        <option value = "100+">100 a viac</option>
                    </select>
            </div>

            <!-- <input type = "submit" value = "Odoslat" id = "reg"> -->
        </form>
    </div>
</template>
 
 <script>
 export default ({
     name: "FormPage",
     components: {
 },
     data() {
         return {}
     },
     methods: {
        other() {
            if (document.getElementById("opt").selected) {
                document.getElementById("checked").style.display = "block";
            }

            else {
                document.getElementById("checked").style.display = "none";
            }
        }
     }
 })
 </script>
 
 <style scoped>
    .formbg {
        background-color: white;
        padding: 2em;
        border: 6px #2395e7 solid;
        border-radius: 16px;
    }

    .cont {
    justify-content: center;
    display: flex;
    flex-wrap: wrap;
    text-align: center;
    font-family:'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
}

.form_group {
    margin-bottom: 2rem;
    justify-content: center;
    display: flex;
    flex-wrap: wrap;
    position: relative;
}

.form_group > i {
    position: absolute;
    left: 20px;
    top: 17px;
    scale: 165%;
}

.form_group > input,
.form_group > select {
    padding-left: 60px;
}

.form_group > select {
    width: 445px;
}

.form_align {
    border-radius: 25px;
    height: 55px;
    width: 385px;
    font-size: 20px;
    border: 1px solid rgb(116, 162, 255);
    background-color:rgb(154, 202, 251);
    color: white;
}

#reg {
    border-radius: 15px;
    height: 35px;
    width: 125px;
    font-size: 20px;
    border: 1px solid rgb(80, 80, 80);
    background-color:rgb(60, 161, 255);
    color: white;
}

::placeholder {
    opacity: 1;
}
 </style>