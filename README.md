# 💝 Convite?

> Site interativo de convite onde o botão **"Não"** foge do cursor — e só resta o **"Sim"**.

![HTML](https://img.shields.io/badge/HTML5-E34F26?style=flat&logo=html5&logoColor=white)
![CSS](https://img.shields.io/badge/CSS3-1572B6?style=flat&logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat&logo=javascript&logoColor=black)
![License](https://img.shields.io/badge/license-MIT-green?style=flat)

---

## ✨ Demo

Abra o arquivo `index.html` no navegador — sem servidor, sem dependências, funciona offline.

---

## 🎮 Como funciona

1. A pessoa abre o site e vê a pergunta **"Quer jantar comigo?"**
2. Toda vez que ela tenta clicar em **"Não"**, o botão **foge para uma posição aleatória**
3. O emoji central vai mudando de expressão a cada tentativa frustrada 🤔 → 😅 → 🥺 → 😭
4. Uma legenda de zoeira aparece embaixo, ficando cada vez mais dramática
5. Ao clicar em **"Sim"**, uma chuva de corações e emojis celebra a resposta certa 🎉

---

## 🗂️ Estrutura

```
.
└── index.html   # tudo em um único arquivo (HTML + CSS + JS)
```

O projeto é **zero dependências** — apenas duas fontes do Google Fonts carregadas via CDN (`Fredoka One` e `Nunito`).

---

## 🎨 Visual

- Fundo escuro com **orbs de luz neon** (vermelho e roxo) pulsando
- Card central com **glassmorphism** (backdrop-filter blur)
- Título com **gradiente laranja/neon**
- Emoji flutuando em animação suave
- Chuva de confete ao confirmar o "Sim"

---

## 🛠️ Personalização

Tudo editável direto no `index.html`:

### Texto da pergunta
```html
<!-- linha ~210 -->
<h1>Quer jantar comigo?</h1>
```

### Mensagem de confirmação (tela do "Sim")
```html
<!-- seção "TELA 2: confirmação" -->
<p>Combinado então! ❤️</p>
<p>Te chamo pra combinar o horário 😍</p>
```

### Frases de zoeira do botão "Não"
```js
// array captions no <script>
const captions = [
  '',
  'hm, tentou apertar o Não? 😅',
  'o botão fugiu de você kkk',
  // adicione mais frases aqui...
];
```

### Cores
Edite as variáveis no topo do `<style>`:
```css
/* orbs de fundo */
.orb1 { background: #c0392b; }   /* vermelho */
.orb2 { background: #7d2d8e; }   /* roxo     */

/* botão Sim */
.btn-sim { background: linear-gradient(135deg, #ff6b35, #c0392b); }
```

---

## ♿ Acessibilidade

- Respeita `prefers-reduced-motion` — animações desativadas automaticamente para quem configurou isso no sistema
- Região do caption usa `aria-live="polite"` para leitores de tela
- Funciona no **celular** (eventos de toque no botão "Não" também fazem ele fugir)

---

## 🚀 Como usar

```bash
# clone o repositório
git clone https://github.com/seu-usuario/quer-jantar-comigo.git

# abra no navegador
open index.html
# ou arraste o arquivo para o navegador
```

Ou hospede de graça no **GitHub Pages**, **Netlify** ou **Vercel** — é um arquivo estático puro.

---

## 📄 Licença

MIT — use à vontade, mande pra pessoa certa e boa sorte. 🍀
