# 🧩 Ever's Maze — Conheça a Ever!

[![▶ Jogue Online](https://img.shields.io/badge/▶_Jogar_Labirinto-8b5cf6?style=for-the-badge&logo=github&logoColor=white&labelColor=8b5cf6&color=white)](https://everferreira.github.io/ever-adventure/)
[![HTML5](https://img.shields.io/badge/HTML5-E34F26?logo=html5)](https://developer.mozilla.org/pt-BR/docs/Web/HTML)

**Um labirinto interativo no navegador — navegue pelos desafios e conheça um pouco sobre mim enquanto joga.**

👉 **Jogue agora:** [everferreira.github.io/ever-adventure](https://everferreira.github.io/ever-adventure/)

---

## 🎯 Pra que isso existe?

> Este sistema ajuda **recrutadores e visitantes do meu portfólio** a **conhecerem minha personalidade e habilidades** de forma divertida, **sem ler um texto estático**.

Em vez de um "Sobre Mim" tradicional, transformei a apresentação num jogo de labirinto com fases. Cada área revela um aspecto diferente — formação, experiência, tecnologias — de forma interativa.

É a diferença entre **falar** que você é criativa e **mostrar** que é criativa.

---

## 🎮 Como jogar

1. Acesse: [https://everferreira.github.io/ever-adventure/](https://everferreira.github.io/ever-adventure/)
2. Use as **setas do teclado** (↑ ↓ ← →) para mover o personagem
3. Navegue até a **saída** de cada fase
4. Cada fase concluída revela um fato ou habilidade

Sem instalação — funciona direto no navegador, no PC ou celular.

---

## 🛠 Tecnologias

| Tecnologia | Por quê |
|---|---|
| **HTML5 + Canvas** | Renderização 2D do labirinto, personagem e colisões |
| **CSS3** | Estilização com gradientes, glassmorphism e responsividade |
| **JavaScript puro** | Lógica do jogo, detecção de colisão por matriz, controle de fases |
| **GitHub Pages** | Deploy gratuito sem backend |

---

## 🧱 Decisões Técnicas

| Problema | Decisão | Resultado |
|---|---|---|
| O personagem atravessava paredes em cantos | Implementei colisão por matriz booleana (cada parede é uma célula da matriz `map[y][x]`) | Movimento fluido em 4 direções sem vazar paredes |
| Precisava de múltiplos mapas sem complicar o código | Usei array de mapas com transição por fade
entre fases | Experiência contínua sem reload |
| Jogo precisava carregar rápido (sem libs externas) | Zero dependências — HTML + CSS + JS inline | Carrega em <1s, funciona offline |

---

## 🚀 Deploy

O projeto é estático (HTML puro) e deployado via GitHub Pages a partir da branch `main`.

Automatizado? Sim — qualquer push na `main` dispara o workflow [pages.yml](.github/workflows/pages.yml).

---

## 📂 Estrutura

```
ever-adventure/
├── index.html   # Jogo completo (HTML + CSS + JS embutidos)
└── .github/
    └── workflows/
        └── pages.yml   # Deploy automático
```

---

## 💡 Próximos passos

- [ ] Adicionar mais fases com desafios de lógica
- [ ] Versão mobile com controles touch
- [ ] Ranking de tempo para completar o labirinto
- [ ] Easter eggs escondidos nas paredes

---

<div align="center">

Feito com 💜 por [Ever Ferreira](https://github.com/everferreira)

</div>