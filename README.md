<!DOCTYPE html>
<html lang="pt-br">
<head>
    <meta charset="UTF-8">
    <meta http-equiv="X-UA-Compatible" content="IE=edge">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Login</title>
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
