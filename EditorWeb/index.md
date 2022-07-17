<h1>Editeur en ligne</h1>
Merci d'ajouter avec chaque changement de lignes "%0A" pour que l'éditeur sache que l'on change de ligne.
<input type="button" id="print" onClick="printPage();" value="Imprimer" />
<textarea id="text" name="text" rows="60" cols="80"></textarea>

<script src="https://code.jquery.com/jquery-3.6.0.min.js" integrity="sha256-/xUj+3OJU5yExlq6GSYGSHk7tPXikynS7ogEvDej/m4=" crossorigin="anonymous"></script>
<script type="text/javascript">
    var text = "";

    $(document).ready(function(){
        const str = window.location.href;

        const words = str.split('#');
        $("#text").val(decodeURI(words[1]));
        text = decodeURI(words[1]);
    });

    $("#text").change(function(){
        text = $("#text").val();
        location.href="#"+text;
    });

    function printPage() {
        location.href="print.html#"+text;
    }
</script>
