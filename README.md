<html>
    <head>
        <title>Meu primeiro HTML</title>
        <link rel="stylesheet" href="index.css">

</head>
    <body>
    
    <style>
    body {
    font-family: Arial, sans-serif;
    background-color: rgb(29, 29, 29);
}

h1 {
    text-align: center;
    margin-top: 50px;
}

.formulario {
    width: 800px;
    margin: 0 auto;
    border: 1px solid white;
    padding: 10px;
    border-radius: 5px;
    box-shadow: 0px 0px 5px;
    background-color: rgb(90, 90, 90);
}

label {
    display: block;
    margin-bottom: 10px;
    font-family: sans-serif;
    color: aliceblue;
    font-weight: bold;

}

label2 {

    margin-bottom: 10px;
    font-family: sans-serif;
    color: aliceblue;
    font-weight: bold;

}

input {
    margin-bottom: 10px;
}

input[type="number"] {
    width: 100%;
    border-radius: 10px;
    border: 1px solid rgb(154, 154, 154);
    margin-bottom: 10px;
    padding: 5px;
}

input[type="text"] {
    border-radius: 10px;
    border: 1px solid rgb(154, 154, 154);
    margin-bottom: 10px;
    padding: 5px;
}

button {
    width: 100%;
    background-color: rgb(33, 192, 33);
    border: none;
    font-size: 16px;
    padding: 5px;
    border-radius: 5px;
    font-weight: bold;
    cursor: pointer;

}

#resultado {
    text-align: center;
    font-weight: bold;
    font-size: 20px;
    margin-top: 20px;
}
    
    
    <style>
    
    
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
