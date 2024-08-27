<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Planejamento de eventos de futebol</title>
    <style>
        body {
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            height: 100vh;
            margin: 0;
            background-color: #f0f0f0;
            font-family: Arial, sans-serif;
        }
        .container {
            display: flex;
            flex-direction: column; /*organiza verticalmente*/
            align-items: center; /*organiza centralmente*/
        }
        .pos {
            text-align: left;
            margin-bottom: 15px; 
            margin-top: 15px; 
            margin-left: -350px/* Espaco das imagens de cima e de baixo em relacao ao lado */
        }
        .img {
            width: 270px; /* largura das imagens */
            height: 270px; /* Novo tamanho das bolas */
            border-radius: 50%;
            object-fit: cover;
            transition: transform 0.3s; /* Transicao suave para fica mais bonito o hoover */
        }
        .pos.meio {
            display: flex;
            align-items: center;
            position: relative; /* Nao mexe o titulo quando mexe a imagem do meio */
            margin-bottom: 30px; 
            margin-top: 30px;
            margin-left: -850px/* Espaco entre a imagem do meio em relacao as outras imagens */
        }
        .img:hover { /*imagens sobem*/ 
            transform: translateY(-10px);
        }
        .h1 { /* fonte do titulo de cima*/
            font-size: 35px;
            font-weight: bold;
            margin-bottom: 10px; /* Espaco entre o texto e a imagem */
            color: 	#4169E1; /* cor da parte de cima*/
        }
        .h2 {
            font-size: 27px;
            font-weight: bold;
            margin-bottom: 10px; 
        }
        .titulo1 {
            position: absolute; /*Nao mexe o titulo quando mexe a imagem do meio */
            top: 120px;
            left: -80px; /* titulo fica a direita da imagem */
            margin-left: 600px; /* Espaco da imagem e o titulo em relacao a esquerda*/
            margin-right: 100px; /* Espaco da imagem e o titulo em relacao a direita, bobao ta literalmente escrito "right"*/
            white-space: nowrap; /*texto não quebra a linha*/
        }
        .titulo2 {
            position: absolute; 
            bottom: 60px;
            left: -10px; 
            margin-left: 600px; 
            white-space: nowrap; 
        }
    </style>
</head>
<body>
    <div class="container">
        <div class="pos">
            <a href="equipamento.html" target="_blank">
                <img src="equipamento.jpg" alt="Imagem 1" class="img">
            </a>
        </div>
        <div class="pos meio">
            <a href="equipes.html" target="_blank">
                <img src="equipe.jpg" alt="Imagem 2" class="img">
            </a>
            <div class="titulo1">
                <div class="h1">Planejamento de Eventos de Futebol, respectivamente: </div><p></p>
            </div>
                <div class="titulo2">
                <div class="h2">Equipamento Necessário, Equipes, Itens de Hospitalidade</div>
            </div>
        </div>
        <div class="pos">
            <a href="hospitalidade.html" target="_blank">
                <img src="estadio.jpg" alt="Imagem 3" class="img">
            </a>
        </div>
    </div>
</body>
</html>
