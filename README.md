# PokéGuide Pokémon

Projeto web em uma única página para montar time, consultar Pokédex e descobrir onde capturar Pokémon, usando dados da PokeAPI.

<p align="center">
  <img src="./web/src/assets/hero.png" alt="Preview do PokéGuide" width="920" />
</p>

## Demo

- GitHub Pages: (adicione o link após o deploy)

## O que tem no app

- **Time**: monte e gerencie seu time (até 6), com status de capturado/não capturado e seleção de moves.
- **Batalha**: recomenda o melhor membro do time contra um oponente (Pokémon ou Boss).
- **Pokédex**: lista com busca e detalhe do Pokémon selecionado.
- **Captura**: mostra onde e como capturar no jogo escolhido (encontros por local).
- **Tipos**: consulta rápida de tipos e efetividade.

## Stack

- React 18 (via CDN) + JSX (Babel in-browser)
- TailwindCSS (via CDN)
- PokeAPI (https://pokeapi.co)

## Rodando localmente

Este repositório é pensado para funcionar como **um arquivo só**: [index.html](index.html).

- Opção 1: abra o arquivo `index.html` no navegador
- Opção 2: suba um servidor local na raiz do projeto (recomendado para evitar bloqueios do browser com `fetch`)
  - Python: `python -m http.server 5173`
  - Node: `npx serve .`

## Deploy no GitHub Pages

O deploy está configurado via GitHub Actions em [.github/workflows/pages.yml](.github/workflows/pages.yml) e publica o `index.html` da raiz.

Passos:

1. Faça push para a branch `main`
2. No GitHub: **Settings → Pages → Build and deployment → Source: GitHub Actions**
3. Aguarde o workflow “Deploy to GitHub Pages” finalizar e use a URL gerada

## Estrutura do repositório

- `index.html`: app principal (SPA em arquivo único)
- `.github/workflows/pages.yml`: pipeline de deploy no GitHub Pages
- `web/`: pasta auxiliar (inclui assets como a imagem do preview)

## Observações

- O app depende de internet (CDNs + PokeAPI).
- A PokeAPI pode ficar lenta/indisponível em alguns momentos; o app usa cache para reduzir requisições.

## Créditos

- Dados: PokeAPI
- Sprites/Imagens: PokeAPI e Pokémon Showdown (sprites de treinadores)
