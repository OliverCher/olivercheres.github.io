# olivercheres.github.io
formulaire
<!DOCTYPE html>
<html>


<h1 style="font-family:fantasy;">
	<center><u>Test De Personalite
</h1>
<h2 style="font-family:fantasy;">
	<center> Test a Multichoix
</h2>
<h3></h3>

<body style="background-color:	SkyBlue ;">
	<form>
		<img src="persone.png" alt="persone" width="100" height="60">
  <head>
    <meta charset="utf-8">
    <meta name="viewport" content="width=device-width">
    <title>repl.it</title>
    <link href="style.css" rel="stylesheet" type="text/css" />
  </head>

<body>
  <br>
1-Aimez vous prendre le cafe le matin ou vous n'en prenez pas? 
   <br>
    <label for="selQuestion1">Multichoix:</label>
<select id="selQuestion1">
<option value="Cafe">Café</option>
<option value="Pas de cafe">Pas de café</option>
</select>
<br>
<br>
2-Vous préferez faire quoi:
<br>
<label for="selQuestion2">Multichoix:</label>
<select id="selQuestion2">
<option value="Dessiné">Dessiné</option>
<option value="Faire du sport">Faire du sport</option>
</select>
<br>
<br>
3-Est tu quelqu'un qui aime socialisez:
<br>
<label for="selQuestion3">Multichoix:</label>
<select id="selQuestion3">
<option value="Oui">Oui</option>
<option value="Non"> Non </option>
</select>
<br>
<br>
4-Lors d'un évenement qui regroupe beaucoup de personne ou vous vous trouvé:
<br>
<label for="selQuestion4">Multichoix:</label>
<select id="selQuestion4">
<option value="Millieu">Millieu</option>
<option value="Côté"> Côté </option>
</select>
<br>
<br>
5-Lequel de base que vous le plus doue: 
<br>
<label for="selQuestion5">Multichoix:</label>
<select id="selQuestion5">
<option value="La precision">La precision(chef, chasseur etc...)</option>
<option value="Le travail manuel"> Le travail manuel(ingénieur, pompiers etc...) </option>
</select>
<br>
<br>
6-Est ce que vous etes nerveux lors des presentation a l'orale?
<br>
<label for="selQuestion6">Multichoix:</label>
<select id="selQuestion6">
<option value="Oui"> Oui </option>
<option value="Non"> Non </option>
</select>
<br>
<br>
7-Participe-tu en classe?: 
<br>
<label for="selQuestion7">Multichoix:</label>
<select id="selQuestion7">
<option value="oui">oui</option>
<option value="non"> non </option>
</select>
<br>
<br>
8-On vous a déjà dit que vous étiez "trop intense"?
<br>
<label for="selQuestion8">Multichoix:</label>
<select id="selQuestion8">
<option value="oui">oui</option>
<option value="non"> non </option>
</select>
<br>
<br>
9- Aimez vous plus sortir que de rester chez vous?
<br>
<label for="selQuestion9">Multichoix:</label>
<select id="selQuestion9">
<option value="oui">oui</option>
<option value="non"> non </option>
</select>
<br>
<br>
<br>
<input type="button" id="btnSoumet" onclick="confirme()"  value="Soumettre le Teste">
<br>
<input type="button" id="btnSoumet" onclick="rezet()"  value="Essayer de nouveau">
<script>
function rezet(){
  var restart = window.location.reload();
        document.body.innerHTML = restart;
}

function confirme() {
  var question1 = document.getElementById("selQuestion1").selectedIndex ;
  var question2 = document.getElementById("selQuestion2").selectedIndex ;
 var question3 = document.getElementById("selQuestion3").selectedIndex ;
  var question4 = document.getElementById("selQuestion4").selectedIndex ;
var question5 = document.getElementById("selQuestion5").selectedIndex ;
var question6 = document.getElementById("selQuestion6").selectedIndex ;
var question7 = document.getElementById("selQuestion7").selectedIndex ;
var question8 = document.getElementById("selQuestion8").selectedIndex ;
var question9 = document.getElementById("selQuestion9").selectedIndex ;
  //tableau 
  var tblPart1 = [ 
    [ "cafe", 0],//1, 2
    ["Pas de cafe", 1]//3,4 
  ];
  var tblPart2 = [
    ["dessiné" , 0],
    ["faire du sport", 1]
  ];
  var tblPart3 = [
    ["Oui" , 0],
    ["Non", 1]
  ];
   var tblPart4 = [
    ["Côté" , 0],
    ["Millieu", 1]
  ];
  var tblPart5 = [
    ["La precision" , 0],
    ["Le travail manuel", 1]
  ];
  var tblPart6 = [
    ["Oui", 0],
    ["Non", 1]
  ];
  var tblPart7 = [
    ["Oui", 0],
    ["Non", 1]
  ];
  var tblPart8 = [
    ["Oui", 0],
    ["Non", 1]
];
  var tblPart9 = [
    ["Oui", 0],
    ["Non", 1]
];
      var point1 = tblPart1[question1][1];
      var point2 = tblPart2[question2][1];
      var point3 = tblPart3[question3][1];
      var point4 = tblPart4[question4][1];
      var point5 = tblPart5[question5][1];
      var point6 = tblPart6[question6][1];
      var point7 = tblPart7[question7][1];
      var point8 = tblPart8[question8][1];
      var point9 = tblPart9[question9][1];

      var  valeur = point1 + point2 + point3 + point4 + point5 + point6 + point7 + point8 +point9;
      if (valeur <= 4 ){
        alert("Vous de personalite introverti qui est personne qui est renfermé sur lui-meme mais et qui a du mal socialisez.")
      }
      else if (valeur > 4){
        alert("Vous de personalite extraverti vous etes tres souvent le centre de l'attention vous faire des amis est devenu seconde nature pour vous.")
      }
      console.log(valeur)
      for (let i= 1; i <= 1; i++){
        alert("Vous avez teminez bravo!!!");
      }
   }  //fin fonction confirm
          </script>
           </form>
  </body>
</html>
