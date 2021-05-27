# projetoFinanc
function saldoPositivo(capitalDeGiro,fixoDeCaixa, vendastotal, vendasLiquido, despesas, lucro, CalcStatus){

vendasLiquido = Vendas - despesas;
vendas = vendas - fixoDeCaixa; 
  totalBruto = vendas + fixoDeCaixa + despesas;
  vendasLiquido = vendas - fixoDeCaixa;
  lucro = totalBruto - fixoDeCaixa - despesas;

if (lucro >= capitalDeGiro ){
 return "Retorno de Investimento";
 
}
if (fixoDeCaixa < 100 ){
return "Erro, fixo de caixa com valor inferior a R$100,00";
}
if (totalBruto <= despesas) {
return 'estamos no Vermelho';
}
if (despesas < totalBruto){
return "temos Lucro";
}
