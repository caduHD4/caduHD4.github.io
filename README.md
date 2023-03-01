<html>
    <head>
        <title>Meu primeiro HTML</title>
        <link rel="stylesheet" href="index.css">

</head>
    <body>
        <h1 style="color: rgb(18, 67, 191)" >Recibo Simples</h1>
        <div class="formulario">
            <label>Valor:</label>
            <input type="number" id="altura" placeholder="00,00" />

            <label>Nome do Pagador:</label>
            <input type="text" id="pagador" placeholder="Digite o nome"/>

            <label>CPF ou CNPJ (opcional): </label>
            <input type="text" id="cpf" placeholder="Informe o cpf ou cnpj" />

            <label>Referente à:</label>
            <input type="text" id="referente" placeholder="Para quem?" />

            <label>Cidade:</label>
            <input type="text" id="cidade" placeholder="Digite a cidade"/>

            <label2>Data:</label>
            <input type="text" id="data" placeholder="Informe a data"/>

            <label>Nome do Emissor:</label>
            <input type="text" id="emissor" placeholder="Digite o nome"/>

            <label>Telefone (opcional):</label>
            <input type="text" id="telefone" placeholder="Informe o número"/>

            <label2>CPF ou CNPJ (opcional):</label>
            <input type="text" id="cpfemi"  placeholder="Informe o cpf ou cnpj"/>
            
            <label>Forma de Pagamento:</label>
                  <input type="radio" id="dinherio" name="fav_language" value="dinheiro">
                  <label2 for="html">Dinheiro</label><br>
                  <input type="radio" id="pix" name="fav_language" value="pix">
                  <label2 for="css">Pix</label><br>
                  <input type="radio" id="cheque" name="fav_language" value="cheque">
                  <label2 for="javascript">Cheque</label>
                  <input type="radio" id="transferencia" name="fav_language" value="transferencia">
                  <label2 for="css">Tranferência/Depósito</label><br>
                  <input type="radio" id="cartao" name="fav_language" value="cartao">
                  <label2 for="javascript">Cartão de crédito/Débito</label>
                
            
            <button onclick="calcular()" id="botao">Gerar Recibo</button>

            <div id="resultado"></div>

        </div>

<script>
    function calcular(){
        var altura = document.getElementById("altura").value;
        var peso = document.getElementById("peso").value;
        var resultado;
        if(altura>0 && peso>0){
            resultado = peso/(altura*altura);
            resultado = resultado.toFixed(2);
        }else{
            resultado ="Legal amigo, sou adivinho agora??💅"
        }
        var divResultado = document.getElementById("resultado");
        divResultado.innerHTML = resultado;
    }

</script>
<script src="index.js"></script>
<body>
</html>
