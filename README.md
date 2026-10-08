```html
<!DOCTYPE html>
<html lang="pt-BR">

<head>

<meta charset="UTF-8">

<meta name="viewport"
      content="width=device-width, initial-scale=1.0">

<title>Achadinhos da Internet</title>

<meta name="description"
      content="Os melhores achadinhos, ofertas e produtos selecionados.">

<style>

/* =========================
   CONFIGURAÇÕES GERAIS
========================= */

* {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
}

body {
    font-family: Arial, Helvetica, sans-serif;
    background: #f5f6f7;
    color: #17212b;
}

a {
    text-decoration: none;
}

button,
input {
    font-family: inherit;
}


/* =========================
   TOPO
========================= */

.topo {
    background: #111b22;
    color: white;
    padding: 18px 5%;
}

.topo-conteudo {
    max-width: 1250px;
    margin: auto;

    display: flex;
    align-items: center;
    gap: 25px;
}


/* LOGO */

.logo {
    display: flex;
    align-items: center;
    gap: 10px;

    min-width: 230px;
}

.logo-icone {
    width: 48px;
    height: 48px;

    background: #ffd000;

    border-radius: 12px;

    display: flex;
    align-items: center;
    justify-content: center;

    font-size: 27px;
}

.logo-texto {
    font-size: 22px;
    font-weight: 800;
    line-height: 1.05;
}

.logo-texto span {
    color: #ffd000;
}


/* =========================
   PESQUISA
========================= */

.pesquisa {
    flex: 1;

    display: flex;

    background: white;

    border-radius: 30px;

    overflow: hidden;
}

.pesquisa input {
    width: 100%;

    border: none;

    outline: none;

    padding: 15px 20px;

    font-size: 15px;
}

.pesquisa button {
    width: 60px;

    border: none;

    background: #ffd000;

    font-size: 22px;

    cursor: pointer;
}


/* WHATSAPP TOPO */

.whatsapp-topo {
    color: white;

    display: flex;

    align-items: center;

    gap: 8px;

    font-weight: bold;

    white-space: nowrap;
}

.whatsapp-topo span {
    color: #25d366;
    font-size: 28px;
}


/* =========================
   MENU
========================= */

.menu {
    background: white;

    border-bottom: 1px solid #ddd;
}

.menu-conteudo {
    max-width: 1250px;

    margin: auto;

    display: flex;

    overflow-x: auto;
}

.menu a {
    padding: 17px 20px;

    color: #222;

    font-weight: bold;

    white-space: nowrap;
}

.menu a:hover {
    background: #fff4b8;
}


/* =========================
   BANNER
========================= */

.banner {
    max-width: 1250px;

    margin: 20px auto;

    padding: 45px;

    border-radius: 20px;

    background: linear-gradient(
        120deg,
        #ffd000,
        #ffb000
    );

    position: relative;

    overflow: hidden;
}

.banner h2 {
    font-size: 42px;

    max-width: 550px;

    margin-bottom: 12px;
}

.banner p {
    font-size: 18px;

    max-width: 520px;

    margin-bottom: 25px;
}

.banner-botao {
    display: inline-block;

    background: #111b22;

    color: white;

    padding: 15px 25px;

    border-radius: 30px;

    font-weight: bold;
}

.banner-produtos {
    position: absolute;

    right: 40px;

    bottom: 0;

    font-size: 130px;
}


/* =========================
   BENEFÍCIOS
========================= */

.beneficios {
    max-width: 1250px;

    margin: 20px auto;

    background: white;

    border-radius: 15px;

    padding: 20px;

    display: grid;

    grid-template-columns:
        repeat(4, 1fr);

    gap: 15px;
}

.beneficio {
    display: flex;

    align-items: center;

    gap: 12px;

    font-size: 14px;
}

.beneficio-icon {
    font-size: 28px;
}


/* =========================
   CONTEÚDO
========================= */

.container {
    max-width: 1250px;

    margin: auto;

    padding: 20px;
}

.titulo {
    display: flex;

    justify-content: space-between;

    align-items: center;

    margin-bottom: 18px;
}

.titulo h2 {
    font-size: 26px;
}


/* =========================
   CATEGORIAS
========================= */

.categorias {
    display: grid;

    grid-template-columns:
        repeat(6, 1fr);

    gap: 12px;

    margin-bottom: 40px;
}

.categoria {
    background: white;

    border-radius: 14px;

    padding: 20px 10px;

    text-align: center;

    cursor: pointer;

    border: 1px solid #eee;

    transition: .2s;
}

.categoria:hover {
    transform: translateY(-3px);

    border-color: #ffd000;
}

.categoria-icon {
    font-size: 42px;

    margin-bottom: 8px;
}

.categoria strong {
    font-size: 14px;
}


/* =========================
   PRODUTOS
========================= */

.produtos {
    display: grid;

    grid-template-columns:
        repeat(4, 1fr);

    gap: 18px;
}

.produto {
    background: white;

    border-radius: 15px;

    overflow: hidden;

    border: 1px solid #e4e4e4;

    transition: .2s;
}

.produto:hover {
    transform: translateY(-4px);

    box-shadow:
        0 10px 25px
        rgba(0,0,0,.10);
}

.produto-imagem {
    height: 230px;

    background: #fafafa;

    display: flex;

    align-items: center;

    justify-content: center;

    font-size: 100px;

    position: relative;
}

.etiqueta {
    position: absolute;

    top: 12px;

    left: 12px;

    background: #e52323;

    color: white;

    padding: 6px 10px;

    border-radius: 6px;

    font-size: 12px;

    font-weight: bold;
}

.info {
    padding: 15px;
}

.info h3 {
    font-size: 16px;

    margin-bottom: 8px;

    min-height: 38px;
}

.descricao {
    color: #777;

    font-size: 13px;

    min-height: 35px;
}

.estrelas {
    color: #ffb900;

    margin: 10px 0;

    font-size: 14px;
}

.preco {
    font-size: 22px;

    font-weight: bold;

    margin-bottom: 12px;
}

.botao-oferta {
    display: block;

    width: 100%;

    text-align: center;

    background: #ffd000;

    color: #111;

    padding: 13px;

    border-radius: 8px;

    font-weight: bold;
}

.botao-oferta:hover {
    background: #ffbd00;
}


/* =========================
   WHATSAPP
========================= */

.whatsapp-box {
    margin: 45px 0;

    background:
        linear-gradient(
            120deg,
            #075e54,
            #128c7e
        );

    color: white;

    border-radius: 18px;

    padding: 25px;

    display: flex;

    justify-content: space-between;

    align-items: center;
}

.whatsapp-box h2 {
    margin-bottom: 5px;
}

.whatsapp-botao {
    background: #25d366;

    color: white;

    padding: 14px 25px;

    border-radius: 30px;

    font-weight: bold;
}


/* =========================
   RODAPÉ
========================= */

footer {
    background: #111b22;

    color: #ccc;

    padding: 40px 20px;
}

.footer-conteudo {
    max-width: 1250px;

    margin: auto;

    display: grid;

    grid-template-columns:
        2fr 1fr 1fr 1fr;

    gap: 30px;
}

footer h3 {
    color: white;

    margin-bottom: 12px;
}

footer p,
footer a {
    color: #bbb;

    font-size: 13px;

    line-height: 1.8;
}

.copyright {
    max-width: 1250px;

    margin: 30px auto 0;

    padding-top: 20px;

    border-top: 1px solid #333;

    font-size: 12px;
}


/* =========================
   RESPONSIVO
========================= */

@media (max-width: 900px) {

    .topo-conteudo {
        flex-wrap: wrap;
    }

    .logo {
        min-width: auto;
    }

    .pesquisa {
        order: 3;

        width: 100%;
    }

    .banner-produtos {
        opacity: .25;
    }

    .beneficios {
        grid-template-columns:
            repeat(2, 1fr);
    }

    .categorias {
        grid-template-columns:
            repeat(3, 1fr);
    }

    .produtos {
        grid-template-columns:
            repeat(2, 1fr);
    }

    .footer-conteudo {
        grid-template-columns:
            repeat(2, 1fr);
    }
}


@media (max-width: 600px) {

    .topo {
        padding: 15px;
    }

    .logo-texto {
        font-size: 19px;
    }

    .whatsapp-topo {
        margin-left: auto;

        font-size: 12px;
    }

    .banner {
        margin: 12px;

        padding: 30px 22px;
    }

    .banner h2 {
        font-size: 30px;
    }

    .banner p {
        font-size: 15px;
    }

    .banner-produtos {
        display: none;
    }

    .beneficios {
        margin: 12px;

        grid-template-columns:
            1fr 1fr;

        padding: 15px;
    }

    .beneficio {
        font-size: 11px;
    }

    .categorias {
        grid-template-columns:
            repeat(3, 1fr);
    }

    .categoria {
        padding: 14px 5px;
    }

    .categoria-icon {
        font-size: 30px;
    }

    .categoria strong {
        font-size: 11px;
    }

    .produtos {
        grid-template-columns:
            1fr 1fr;

        gap: 10px;
    }

    .produto-imagem {
        height: 160px;

        font-size: 65px;
    }

    .info {
        padding: 10px;
    }

    .info h3 {
        font-size: 14px;
    }

    .preco {
        font-size: 18px;
    }

    .botao-oferta {
        font-size: 12px;

        padding: 11px 5px;
    }

    .whatsapp-box {
        flex-direction: column;

        text-align: center;

        gap: 20px;
    }

    .footer-conteudo {
        grid-template-columns: 1fr;
    }
}

</style>

</head>


<body>


<!-- =========================
     CABEÇALHO
========================= -->

<header class="topo">

<div class="topo-conteudo">


<div class="logo">

<div class="logo-icone">
🛒
</div>

<div class="logo-texto">
Achadinhos<br>
<span>da Internet</span>
</div>

</div>


<div class="pesquisa">

<input
type="text"
id="campoPesquisa"
placeholder="O que você está procurando?"
onkeyup="pesquisarProdutos()">

<button onclick="pesquisarProdutos()">
🔎
</button>

</div>


<a
class="whatsapp-topo"
href="https://wa.me/SEUNUMERO"
target="_blank">

<span>◉</span>

Fale conosco<br>
no WhatsApp

</a>


</div>

</header>


<!-- =========================
     MENU
========================= -->

<nav class="menu">

<div class="menu-conteudo">

<a href="#">🏠 Início</a>

<a href="#produtos">📱 Eletrônicos</a>

<a href="#produtos">🏠 Casa e Cozinha</a>

<a href="#produtos">💄 Beleza</a>

<a href="#produtos">⚽ Esporte</a>

<a href="#produtos">👕 Moda</a>

<a href="#produtos">🔧 Ferramentas</a>

</div>

</nav>


<!-- =========================
     BANNER
========================= -->

<section class="banner">

<h2>
Os melhores<br>
achadinhos da Internet
</h2>

<p>
Produtos selecionados, ofertas e novidades
que encontramos para você.
</p>

<a
href="#produtos"
class="banner-botao">

🔥 VER OFERTAS

</a>

<div class="banner-produtos">
📱 🎧 📺
</div>

</section>


<!-- =========================
     BENEFÍCIOS
========================= -->

<section class="beneficios">

<div class="beneficio">

<div class="beneficio-icon">🚚</div>

<div>
<strong>Entrega rápida</strong><br>
Produtos enviados pelo Mercado Livre
</div>

</div>


<div class="beneficio">

<div class="beneficio-icon">🛡️</div>

<div>
<strong>Compra segura</strong><br>
Compra realizada no Mercado Livre
</div>

</div>


<div class="beneficio">

<div class="beneficio-icon">🏷️</div>

<div>
<strong>Ofertas todos os dias</strong><br>
Achadinhos selecionados
</div>

</div>


<div class="beneficio">

<div class="beneficio-icon">⭐</div>

<div>
<strong>Produtos populares</strong><br>
Selecionados para você
</div>

</div>

</section>


<!-- =========================
     CONTEÚDO
========================= -->

<main class="container">


<div class="titulo">

<h2>
📂 Categorias
</h2>

</div>


<!-- CATEGORIAS -->

<section class="categorias">

<div class="categoria"
onclick="filtrarCategoria('eletronicos')">

<div class="categoria-icon">📱</div>

<strong>Eletrônicos</strong>

</div>


<div class="categoria"
onclick="filtrarCategoria('casa')">

<div class="categoria-icon">🍳</div>

<strong>Casa e Cozinha</strong>

</div>


<div class="categoria"
onclick="filtrarCategoria('beleza')">

<div class="categoria-icon">💄</div>

<strong>Beleza</strong>

</div>


<div class="categoria"
onclick="filtrarCategoria('esporte')">

<div class="categoria-icon">👟</div>

<strong>Esporte</strong>

</div>


<div class="categoria"
onclick="filtrarCategoria('moda')">

<div class="categoria-icon">👕</div>

<strong>Moda</strong>

</div>


<div class="categoria"
onclick="filtrarCategoria('ferramentas')">

<div class="categoria-icon">🔧</div>

<strong>Ferramentas</strong>

</div>

</section>


<!-- =========================
     PRODUTOS
========================= -->

<div
class="titulo"
id="produtos">

<h2>
🔥 Produtos em destaque
</h2>

</div>


<section class="produtos">


<!-- PRODUTO 1 -->

<article
class="produto"
data-nome="fone bluetooth jbl"
data-categoria="eletronicos">

<div class="produto-imagem">

<span class="etiqueta">
Mais vendido
</span>

🎧

</div>

<div class="info">

<h3>
Fone Bluetooth JBL
</h3>

<p class="descricao">
Fone sem fio para música e chamadas.
</p>

<div class="estrelas">
★★★★★
</div>

<div class="preco">
R$ 99,90
</div>

<a
href="COLE_SEU_LINK_AQUI"
class="botao-oferta"
target="_blank"
rel="noopener">

🛒 VER OFERTA

</a>

</div>

</article>


<!-- PRODUTO 2 -->

<article
class="produto"
data-nome="air fryer"
data-categoria="casa">

<div class="produto-imagem">

<span
class="etiqueta"
style="background:#16a34a">

Oferta especial
</span>

🍳

</div>

<div class="info">

<h3>
Air Fryer
</h3>

<p class="descricao">
Praticidade para sua cozinha.
</p>

<div class="estrelas">
★★★★★
</div>

<div class="preco">
R$ 299,90
</div>

<a
href="COLE_SEU_LINK_AQUI"
class="botao-oferta"
target="_blank"
rel="noopener">

🛒 VER OFERTA

</a>

</div>

</article>


<!-- PRODUTO 3 -->

<article
class="produto"
data-nome="smart tv 50 4k"
data-categoria="eletronicos">

<div class="produto-imagem">

<span class="etiqueta">
Oferta
</span>

📺

</div>

<div class="info">

<h3>
Smart TV 50" 4K
</h3>

<p class="descricao">
Imagem 4K e sistema Smart.
</p>

<div class="estrelas">
★★★★★
</div>

<div class="preco">
R$ 1.799,90
</div>

<a
href="COLE_SEU_LINK_AQUI"
class="botao-oferta"
target="_blank"
rel="noopener">

🛒 VER OFERTA

</a>

</div>

</article>


<!-- PRODUTO 4 -->

<article
class="produto"
data-nome="smartphone celular"
data-categoria="eletronicos">

<div class="produto-imagem">

<span
class="etiqueta"
style="background:#16a34a">

Lançamento
</span>

📱

</div>

<div class="info">

<h3>
Smartphone
</h3>

<p class="descricao">
Celular moderno para o dia a dia.
</p>

<div class="estrelas">
★★★★★
</div>

<div class="preco">
R$ 899,90
</div>

<a
href="COLE_SEU_LINK_AQUI"
class="botao-oferta"
target="_blank"
rel="noopener">

🛒 VER OFERTA

</a>

</div>

</article>


<!-- PRODUTO 5 -->

<article
class="produto"
data-nome="kit maquiagem"
data-categoria="beleza">

<div class="produto-imagem">

💄

</div>

<div class="info">

<h3>
Kit de Maquiagem
</h3>

<p class="descricao">
Kit completo para maquiagem.
</p>

<div class="estrelas">
★★★★★
</div>

<div class="preco">
R$ 79,90
</div>

<a
href="COLE_SEU_LINK_AQUI"
class="botao-oferta"
target="_blank"
rel="noopener">

🛒 VER OFERTA

</a>

</div>

</article>


<!-- PRODUTO 6 -->

<article
class="produto"
data-nome="tenis esportivo"
data-categoria="esporte">

<div class="produto-imagem">

👟

</div>

<div class="info">

<h3>
Tênis Esportivo
</h3>

<p class="descricao">
Confortável para caminhada e treino.
</p>

<div class="estrelas">
★★★★★
</div>

<div class="preco">
R$ 129,90
</div>

<a
href="COLE_SEU_LINK_AQUI"
class="botao-oferta"
target="_blank"
rel="noopener">

🛒 VER OFERTA

</a>

</div>

</article>


<!-- PRODUTO 7 -->

<article
class="produto"
data-nome="camiseta masculina"
data-categoria="moda">

<div class="produto-imagem">

👕 

</div>

<div class="info">

<h3>
Camiseta Masculina
</h3>

<p class="descricao">
Camiseta confortável para o dia a dia.
</p>

<div class="estrelas">
★★★★★
</div>

<div class="preco">
R$ 49,90
</div>

<a
href="COLE_SEU_LINK_AQUI"
class="botao-oferta"
target="_blank"
rel="noopener">

🛒 VER OFERTA

</a>

</div>

</article>


<!-- PRODUTO 8 -->

<article
class="produto"
data-nome="furadeira"
data-categoria="ferramentas">

<div class="produto-imagem">

🔧

</div>

<div class="info">

<h3>
Furadeira Elétrica
</h3>

<p class="descricao">
Ferramenta para trabalhos domésticos.
</p>

<div class="estrelas">
★★★★★
</div>

<div class="preco">
R$ 159,90
</div>

<a
href="COLE_SEU_LINK_AQUI"
class="botao-oferta"
target="_blank"
rel="noopener">

🛒 VER OFERTA

</a>

</div>

</article>


</section>


<!-- =========================
     WHATSAPP
========================= -->

<section class="whatsapp-box">

<div>

<h2>
💬 Precisa de ajuda?
</h2>

<p>
Fale conosco pelo WhatsApp.
</p>

</div>

<a
href="https://wa.me/SEUNUMERO"
target="_blank"
class="whatsapp-botao">

💚 CHAMAR NO WHATSAPP

</a>

</section>


</main>


<!-- =========================
     RODAPÉ
========================= -->

<footer>

<div class="footer-conteudo">


<div>

<h3>
🛒 Achadinhos da Internet
</h3>

<p>
Sua guia de compras online.
</p>

<p>
Selecionamos produtos e ofertas
para facilitar suas compras.
</p>

</div>


<div>

<h3>
Categorias
</h3>

<p>Eletrônicos</p>

<p>Casa e Cozinha</p>

<p>Beleza</p>

<p>Moda</p>

</div>


<div>

<h3>
Atendimento
</h3>

<p>
WhatsApp
</p>

<p>
Fale conosco
</p>

</div>


<div>

<h3>
Informações
</h3>

<p>
Termos de uso
</p>

<p>
Política de privacidade
</p>

<p>
Links de afiliado
</p>

</div>


</div>


<div class="copyright">

© 2026 Achadinhos da Internet — Todos os direitos reservados.

<br><br>

Alguns links desta página podem ser links de afiliado.
Quando você realiza uma compra através deles,
podemos receber uma comissão.

</div>

</footer>


<!-- =========================
     JAVASCRIPT
========================= -->

<script>

/* PESQUISA */

function pesquisarProdutos() {

    const texto =
        document
        .getElementById("campoPesquisa")
        .value
        .toLowerCase();

    const produtos =
        document.querySelectorAll(".produto");

    produtos.forEach(function(produto) {

        const nome =
            produto
            .getAttribute("data-nome")
            .toLowerCase();

        if (nome.includes(texto)) {

            produto.style.display = "block";

        } else {

            produto.style.display = "none";

        }

    });

}


/* FILTRO POR CATEGORIA */

function filtrarCategoria(categoria) {

    const produtos =
        document.querySelectorAll(".produto");

    produtos.forEach(function(produto) {

        const categoriaProduto =
            produto.getAttribute("data-categoria");

        if (categoriaProduto === categoria) {

            produto.style.display = "block";

        } else {

            produto.style.display = "none";

        }

    });

    document
    .getElementById("produtos")
    .scrollIntoView({
        behavior: "smooth"
    });

}

</script>


</body>
</html>
```

