<a href="../"><img src="../back.png" title="Revenir en arrière" alt="Revenir en arrière"></a><br>
<h2>Back&Next</h2>
Back&Next est un système de boutons (un avec précédent, l'autre avec suivant et un bouton OK(optitionnel))<br>
Le principe de fonctionnement est très simple : <br>Il suffit de remplir le formulaire puis d'appuyer sur Générer, de choisir un mode de rendu (Page web complète, Page Php complète, morceau de code) et enfin... Voilà ! (Si vous appuyez sur Page web complète ou Page Php complète, on vous demandera un titre de page Web)<hr><div id="form"><input type="button" value="Ajouter une phase" onClick="add(0);"></div>
<script type="text/javascript" src="/JQuery/jquery.js">
<script type="text/javascript">
    function Add(type) {
        if(type==0){
            $("#form").html($("#form").text()+"<br>II");
        }
    }
</script>