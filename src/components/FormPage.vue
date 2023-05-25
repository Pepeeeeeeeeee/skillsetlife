<template>
    <div class = "formbg">
        <form action = "../php/register.php" method = "post">
            <div class = "form_group">
                <label for = "full_name">Meno a Priezvisko</label>
                <input name = "full_name" type = "text" class = "form_align">
            </div>
            
            <div class = "form_group">
                <label for = "mail">E-Mail</label>
                <input name = "mail" type = "email" class = "form_align">
            </div>
    
            <div class = "form_group">
                <label for = "phone_number">Telefonne cislo</label>
                <input name = "phone_number" type = "text" class = "form_align">
            </div>
    
            <div class = "form_group">
                <label for = "organization">Typ organizacie</label>
                <select name = "organization" class = "form_align">
                    <option value = "Skola" onclick = "other()">Skola</option>
                    <option value = "Firma" onclick = "other()">Firma</option>
                    <option value = "Statna institucia" onclick = "other()">Statna institucia</option>
                    <option value = "Ine" id = "opt" onclick = "other()">Ine</option>
                </select>
            </div>
    
            <div style = "display: none;" class = "form_group" id = "checked">
                <input name = "other" type = "text" class = "form_align">
            </div>
    
            <div class = "form_group">
                <label for = "amount">Priblizny pocet osob v organizacii</label>
                <select name = "amount" class = "form_align">
                    <option value = "1-10">1-10</option>
                    <option value = "10-100">10-100</option>
                    <option value = "100+">100 a viac</option>
                </select>
            </div>

            <!-- <input type = "submit" value = "Register" name = "reg"> -->
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
    .form_group {
    margin-bottom: 1rem;
    }

    .formbg{
        background-color: aquamarine;
    }

    .form_align {
    display: block;
    }
 </style>