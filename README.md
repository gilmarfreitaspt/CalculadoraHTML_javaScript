# CalculadoraHTML_javaScript
Feito em sala de aula foi ultilizado HTML e javaScript
segue abaixo todo o codigo ultilizado

<!DOCTYPE html>
<html lang="pt-pt">
<head>
    <title>Exercício 07 - Javascript</title>
<meta charset="utf-8" />
<script type="text/javascript">

     var num1,num2,resut;
    
  
    
  function ativa(){
      document.getElementById("f1").disabled=false;
      document.getElementById("f2").disabled=false;
      
  }
    function somar(){
    num1= document.getElementById("id1").value; 
    num2= document.getElementById("id2").value;
    var soma = parseInt(num1)+parseInt(num2);
    document.getElementById("id3").value=soma;
     }
    function diminuir(){
    num1= document.getElementById("id1").value; 
    num2= document.getElementById("id2").value;
    var sub = parseInt(num1)-parseInt(num2);
    document.getElementById("id3").value=sub;
    }
    function vezes(){
    num1= document.getElementById("id1").value; 
    num2= document.getElementById("id2").value;
    var multiplic = parseInt(num1)* parseInt(num2);
    document.getElementById("id3").value=multiplic ;
    }
    function dividir(){
    num1= document.getElementById("id1").value; 
    num2= document.getElementById("id2").value;
    var div = parseInt(num1)/ parseInt(num2);
    document.getElementById("id3").value=div ;
    }
    function potencia(){
    num1= document.getElementById("id1").value; 
    num2= document.getElementById("id2").value;
    var pot= Math.pow(num1,num2);
    document.getElementById("id3").value=pot;
    }
    
    
  function desativa(){
      
       document.getElementById("f1").disabled=true;
       document.getElementById("f3").disabled=false;
  }
     
      


</script>
</head>
<body>
    <h1>Calculadora Crest</h1>
    <form name="form1" action="ex6.php" onsubmit="return validar()">
    <table width="30%">
        
 
      <fieldset id="f1" disabled>
     <input type="number" id="id1">
     <input type="number" id="id2">
     <input type="button" onclick=somar() value="+">
     <input type="button" onclick=diminuir() value="-">
     <input type="button" onclick=vezes() value= "*" >
     <input type="button" onclick=dividir() value="/">
     <input type="button" onclick=potencia() value="pot">
     <input type="text" id="id3" readonly>
          
   </fieldset>
            
    <button type="button" id="f3"onclick="ativa()">Ativar</button>
    <button type="button"id="f2" onclick="desativa()" disabled>Desativar</button >   
         
        
       
        
    </table>
    
    </form>

  </body>
</html>
