# jose-jeivyson

<!DOCTYPE html>
<!-- 
Código escrito por jeivyson
-->
<html lang="en">

<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Namora comigo?</title>
</head>

<body>
    <div id="conteudo">
        <h2>Aceita namorar comigo?</h2>
        <div style="margin: auto;width: 170px;">
            <button style="position: fixed;display: block;" class="btn" onclick="Sim()">Não</button>
            <button class="btn" onclick="desvia(this)" onmouseover="desvia(this)" style="position: absolute;">Sim</button>
        </div>
    </div>
</body>
<style>
    #conteudo {
        background: #6508df;
        width: 100%;
        height: 100%;
        position: fixed;
        top: 0;
        left: 0;
        padding: 10px;
        text-align: center;
        font-family: sans-serif;
    }

    .btn {
        background: rgb(0, 0, 0);
        color: white;
        border: none;
        padding: 10px;
        width: 80px;
        border-radius: 5px;
    }
</style>

<script>
    function Sim() {
        alert(" Não quer namorar comigo! :(");
        // redireciona para um URL após clicar no SIM
        location.href = "https://www.youtube.com/watch?v=5hnSlCygsTs";
    }

    function desvia(btn) {
        // btn declarado na função
        btn.style.position = 'absolute';
        btn.style.bottom = geraPosicao(10, 90);
        btn.style.left = geraPosicao(10, 90);
        console.log('opa, desviei...');
    }

    function geraPosicao(min, max) {
        return (Math.random() * (max - min) + min) + "%";
    }

    /* Apague se quiser, isso apenas escreve jeivyson */
    const o = "jeivyson", e = 90, l = "bold"; console.log(`%c${o}`, "font-size: 90px; font-weight: bold; background: linear-gradient(90deg, red, yellow);"), console.log("Tutorial: https://www.youtube.com/watch?v=zxxB9SFh9p4");

</script>

</html>
