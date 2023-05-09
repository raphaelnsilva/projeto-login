<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Login</title>
 <style>
  @charset "UTF-8";

/*
    paleta de cores
    verde: #49a09d
    lilás: #5f2c82
*/

* {
    font-family: system-ui, -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, 'Open Sans', 'Helvetica Neue', sans-serif;
    padding: 0px;
    margin: 0px;
    box-sizing: border-box;
}

body, html {
    background-color: #5f2c82;
    height: 100vh;
    width: 100vw;
}

main {
    position: relative;
    height: 100vh;
    width: 100vw;
}

section#login {
    position: absolute;
    top: 50%;
    left: 50%;
    overflow: hidden; /*oque estiver fora da borda ficara escondido*/

    background-color: white;
    width: 250px;
    height: 540px;
    border-radius: 10px;
    box-shadow: 0px 0px 10px rgba(0, 0, 0, 0.5);

    transition: width .3s, height .3s; /* animação de transição */
    transition-timing-function:none; /*suavisa a animação com o "ease"*/
    transform: translate(-50%, -50%);
}

section#login > div#imagem {
    display: block;
    background: #5f2c82 url(../imagens/porta.jpeg) no-repeat;
    background-size: cover;
    height: 200px;
}

section#login > div#formulario {
    display: block;
    padding: 8px;
}

div#formulario > h1 {
    text-align: center;
    margin-bottom: 10px;
} 

div#forumlario > p {
    font-size: 0.8em;
}

form > input[type=submit] {
    display: block;
    font-size: 1em;
    width: 100%;
    height: 40px;
    background-color: #49a09d;
    color: white;
    border: none;
    border-radius: 5px;
    cursor: pointer;
}

form > input[type=submit]:hover {
    background-color: #316e6c;
}

form > div.campo {
    background-color: #5f2c82;
    border: 2px solid #5f2c82;
    display: block;
    width: 100%;
    height: 40px;
    border-radius: 5px;
    margin: 5px 0px;
}

div.campo >label {
    display: none;
}

div.campo > span {
    color: white;
    font-size: 1.3em;
    width: 40px;
    padding: 5px;
}

div.campo > input {
    background-color: #bfe0df;
    font-size: 1em;
    width: calc(100% - 44.5px);
    height: 100%;
    border: 0px;
    border-radius: 5px;
    transform: translate(-1px);
}

div.campo > input:focus-within {
    background-color: white;
}

form > a.botao {
    display: block;
    text-align: center;
    font-size: 1em;
    width: 100%;
    height: 40px;
    padding-top: 5px;
    margin-top: 5px;
    background-color: white;
    color: #1f4948;
    border: 1px solid #376968;
    border-radius: 7px;
    text-decoration: none;
}

form > a.botao:hover {
    background-color: #61ece78e;
}

form > a.botao > span {
    font-size: 0.8em;
}
 </style>

    <link rel="stylesheet" href="https://fonts.googleapis.com/css2?family=Material+Symbols+Outlined:opsz,wght,FILL,GRAD@20..48,100..700,0..1,-50..200" />

    <link rel="stylesheet" href="estilos/style.css">
    <link rel="stylesheet" href="estilos/query.css">
</head>
<body>
    <main>
        <section id="login">
            <div id="imagem">
                
            </div>
            <div id="formulario">
                <h1>Login</h1>
                <p>Seja bem-vindo(a) novamente, Faça login para acessar sua conta e poder fazer configurações no seu ambiente</p>
                <form action="login.php" method="post" autocomplete="on">
                    <div class="campo">
                        <span class="material-symbols-outlined">person</span>
                       <input type="email" name="login" id="ilogin" placeholder="Seu email" autocomplete="email" required maxlength="30">
                       <label for="ilogin">Login</label> 
                    </div>
                    <div class="campo">
                        <span class="material-symbols-outlined">vpn_key</span>
                        <input type="password" name="senha" id="isenha" placeholder="Sua senha" autocomplete="current-password" required minlength="8" maxlength="20">
                        <label for="isenha">Senha</label>
                    </div>
                    <input type="submit" value="Entrar">
                    <a href="esqueci.html" class="botao">
                        esqueci a senha <span class="material-symbols-outlined">mail</span>
                    </a>
                </form>
            </div>
        </section>
    </main>
</body>
</html>
