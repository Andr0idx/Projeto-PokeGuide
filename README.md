# PokéGuide Pokémon

Projeto web em uma única página para montar time, consultar Pokédex e descobrir onde capturar Pokémon, usando dados da PokeAPI.

![Preview](web/src/assets/hero.png)

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
- Opção 2: suba um servidor local simples na raiz do projeto e acesse no navegador

## Deploy no GitHub Pages

O deploy está configurado via GitHub Actions em [.github/workflows/pages.yml](.github/workflows/pages.yml) e publica o `index.html` da raiz.

Passos:

1. Faça push para a branch `main`
2. No GitHub: **Settings → Pages → Build and deployment → Source: GitHub Actions**
3. Aguarde o workflow “Deploy to GitHub Pages” finalizar e use a URL gerada

## Créditos

- Dados: PokeAPI
- Sprites/Imagens: PokeAPI e Pokémon Showdown (sprites de treinadores)

