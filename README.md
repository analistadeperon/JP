# JP
<div id="root"></div>

<script> DPM
 
 var nome = prompt("Informe o seu nome");
 var sexo = prompt("Informe o seu sexo :'M - Masculino' ou 'F - Femenino'");
 
 if(sexo =="M" || sexo == "m" || sexo == "F" || sexo == "f"){
  var horasTrab = parseInt(prompt("Informe quantas horas vc trabalhou nesse mes!"));
  var salarioBase = parseFloat(prompt("Informe o seu salario Base!")); 
  var horasExtra = horasTrab - 198; 
  var valorHoraExtra = ((salarioBase / 198)*0.30)+(salarioBase /198); 
  var salarioFinal = salarioBase+(horasExtra * valorHoraExtra); 
 
  if(horasTrab == 198){
   document.write("<p>senhor:" + nome +
       "<br />Horas trabalhada:" +horasTrab+
       "<br />Voce teve em horas extras:" +horasExtra+
       "<br />O seu salario e de:"+ salarioFinal);
  }else if(horasTrab > 198){
   document.write("<p>senhor:" + nome +
       "<br />Horas trabalhada:" +horasTrab+
       "<br />Voce teve em horas extras:" +horasExtra+
       "<br />O seu salario e de:"+ salarioBase+
       "<br />O seu salario final eh:"+ salarioFinal);
  }else{
   document.write("<p>senhor:" + nome +
       "<br />Horas trabalhada:" +horasTrab+
       "<br />Voce esta devendo em horas extras:" +horasExtra+
       "<br />O seu salario e de:"+ salarioBase+
       "<br />O seu salario final eh:"+ salarioFinal);
  }
 }else{
  document.write("Codigo do sexo invalido"+
      "De um F5 para continuar!");
 }
</script>
