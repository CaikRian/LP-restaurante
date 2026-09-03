# LP-restaurante

# 🔥 Fumaça

Landing page de um restaurante **fictício** — uma parrilla de brasa viva na Vila Madalena, São Paulo. Projeto de demonstração de front-end: HTML, CSS e JavaScript puros em um único arquivo, sem frameworks, sem build step.

![Hero da página Fumaça](readme_assets/hero.jpg)

## Sobre o projeto

Fumaça foi criado para explorar uma direção de arte fora do piloto automático de "landing page bonita": estética de **cartaz de risograph** — papel kraft, cores de impressão estouradas, tipografia condensada gigante, registro levemente artesanal — em vez do visual clean/minimalista que qualquer gerador de site entrega hoje.

Não existe restaurante real por trás disso. Nome, endereço, cardápio, preços e a equipe são inventados. As fotos usadas são geradas por IA.

## Preview

| Cardápio com filtro | Brasa generativa |
|---|---|
| ![Cardápio](readme_assets/cardapio.jpg) | ![Brasa](readme_assets/brasa.jpg) |

<img src="readme_assets/mobile.jpg" alt="Versão mobile" width="280">

## Destaques técnicos

- **Zero dependências de build** — um único arquivo `.html` autocontido, imagens embutidas em base64. Abre direto no navegador ou em qualquer host estático.
- **Cardápio com filtro interativo** — categorias (Carnes, Acompanhamentos, Bebidas) filtradas em JS puro, sem reload.
- **Elemento generativo em canvas** — uma fileira de brasas acesas que reage à posição do mouse, com leitura de "temperatura" atualizada em tempo real.
- **Cursor customizado em forma de carimbo** — clicar em qualquer lugar da página estampa uma marca "FUMAÇA" que desaparece com fade.
- **Reveals de scroll** via `IntersectionObserver`, sem libs de animação.
- **`prefers-reduced-motion` respeitado** — todas as animações (fogo, marquee, reveals) são desativadas para quem pediu menos movimento no sistema.
- **Responsivo de verdade** — layout recomposto no mobile (não é só empilhar as mesmas colunas); grid substituído por blocos simples abaixo de 860px para evitar bugs de `1fr` no Chromium.

## Stack

- HTML5 + CSS3 (custom properties, `clamp()`, grid, flexbox)
- JavaScript vanilla (sem frameworks, sem dependências externas)
- Fontes: [Anton](https://fonts.google.com/specimen/Anton), [Space Grotesk](https://fonts.google.com/specimen/Space+Grotesk) e [JetBrains Mono](https://fonts.google.com/specimen/JetBrains+Mono), via Google Fonts

## Como rodar

Não precisa de servidor nem instalação — é um arquivo HTML único.

```bash
git clone https://github.com/CaikRian/fumaca.git
cd fumaca
open fumaca-restaurante.html   # macOS
# ou apenas arraste o arquivo para o navegador
```

## Estrutura

```
.
├── fumaca-restaurante.html   # arquivo final, pronto para abrir/publicar
└── readme_assets/            # imagens usadas neste README
```

## Aviso

Este é um **site de demonstração**. O restaurante "Fumaça", seu endereço, cardápio e equipe são fictícios. Todas as fotografias exibidas na página foram **geradas por inteligência artificial** e não retratam um estabelecimento, pratos ou pessoas reais.

## Autor

Feito por [**@CaikRian**](https://github.com/CaikRian).
