# 💝 Nosso Jogo de Palavras

Um web game romântico inspirado no famoso "Wordle" (ou "Termo"), totalmente personalizado para ser um presente inesquecível de aniversário de namoro.

Em vez de palavras aleatórias do dicionário, o jogador deve adivinhar palavras que marcaram a história do casal (lugares, apelidos, gostos pessoais), sempre guiado por uma dica especial a cada rodada.

## 🎮 Como Jogar

O objetivo é descobrir a palavra secreta usando no máximo **6 tentativas**.
Diferente do Wordle tradicional, aqui **as palavras podem ter tamanhos variados** (4, 5, 6 letras, etc.), e o grid se adapta automaticamente!

Após digitar um palpite e apertar "ENVIAR" (ou Enter), as letras giram e mudam de cor para mostrar o quão perto você está da resposta:

* 🟩 **Verde:** A letra está na palavra e na **posição correta**.
* 🟨 **Amarelo:** A letra está na palavra, mas na **posição errada**.
* ⬛ **Cinza (Escuro):** A letra **não faz parte** da palavra.

Fique de olho na **Dica** brilhando no topo da tela para te ajudar a lembrar das memórias do casal!

## ✨ Funcionalidades e Diferenciais

* **Níveis Personalizados:** Sistema de fases onde o jogador avança de uma palavra para a outra.
* **Tamanhos Dinâmicos:** O CSS Grid se adapta automaticamente ao tamanho da palavra configurada (não fica restrito a apenas 5 letras).
* **Teclado Virtual Inteligente:** Teclado na tela que muda de cor conforme os seus palpites, além de suportar digitação pelo teclado físico (PC).
* **Design Moderno:** Interface rica construída com *Glassmorphism* (efeito de vidro fosco) e um fundo gradiente animado.
* **Efeitos Especiais:** Animações 3D ao virar as letras, *shake* ao tentar enviar uma palavra incompleta e chuva de confetes nas vitórias (via `canvas-confetti`).
* **Indicador de Progresso:** Mostra claramente em qual tentativa (ex: "Tentativa 2 de 6") o jogador está, destacando apenas a linha atual.

## 🛠️ Tecnologias Utilizadas

Projeto construído de forma limpa, sem necessidade de *build tools* ou frameworks pesados (100% Front-end estático):

* **HTML5**
* **Tailwind CSS** (via CDN para estilização rápida e responsiva)
* **JavaScript (Vanilla)** (Lógica de estados, verificação de arrays e manipulação do DOM)
* **Canvas Confetti** (Efeitos de celebração)

## 🚀 Como Executar e Personalizar para Você

Você não precisa instalar nada. Para jogar localmente, basta fazer o clone do repositório (ou baixar o código) e abrir o arquivo `index.html` em qualquer navegador.

### Quer fazer a sua própria versão?

Se você achou a ideia legal e quer presentear sua própria pessoa amada, é super fácil alterar as palavras!

1. Abra o arquivo `index.html` no seu editor de código favorito.
2. Desça até a tag `<script>` e procure a variável `const levels = [...]`.
3. Substitua as palavras (`word`) e as dicas (`hint`) pelas suas próprias memórias.
   * *Atenção:* Não use acentos ou espaços nas palavras dentro da variável `word` (ex: use "ITALIA" em vez de "ITÁLIA").

```javascript
const levels = [
    { word: "PRAIA", hint: "Onde fomos no nosso primeiro encontro." },
    { word: "GATOS", hint: "Nossos animais favoritos." }
];
```

## 🌐 Publicação (Deploy)

Este projeto está pronto para o **GitHub Pages**. Basta enviar os arquivos para um repositório público no GitHub, acessar `Settings > Pages`, e ativar o deploy através da branch `main`. Em poucos minutos, seu jogo estará online para você enviar o link como surpresa!

*Feito com muito amor (e muito código) ❤️*