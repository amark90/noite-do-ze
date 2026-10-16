---
name: tasca-grafismo
description: >-
  Guarda o desenho da Tasca do Abílio: um só traço, os retratos em cast/, o balcão
  pintado, e os sítios de publicidade dentro do mundo. Usar ao desenhar, ao
  mexer em paredes, copo, rua, cartaz, placard, ou ao acrescentar uma imagem.
---

# Grafismo — Tasca do Abílio

Um traço só, o dos retratos em `cast/`. Tinta e cel. Sem fotografia por baixo, sem banner por cima, sem segundo estilo no mesmo ecrã.

## O que já está pintado

Adereços em `cast/` como JPG. O magenta de fundo sai. A blusa magenta da Albertina não se apaga. `SOLID` (`paredeTasca`, `paredeFina`, `balcao`) não leva recorte. O copo usa `knockGlass`. O balcão corta 8% em cima e em baixo por causa das barras pretas.

A parede cruza fancy e tasco com `houseMood()`. Revista e não-fiado quando a casa suja. Carta quando a casa está fina. O vidro fica à direita (`GX` 708). Não lhe pôr nada por cima. No balcão a cara fica livre: o balão senta-se ao lado da cabeça, a fila fica atrás e mais baixa, e a caixa de um recado vai na mão, não na cara de quem está à frente.

A rua vê-se de cima, de noite. O chão, as casas e os carros parados são as pinturas em `art/rua/`. Quem anda é uma figura inteira de `art/casa/` (passo de pernas, frente e costas), não um círculo com retrato. O retrato de `cast/` já não vai à cabeça.

A casa rosa, por dentro, é a sala pintada `art/casa/sala.jpg`. Lá anda-se. A mulher, sem nome e vestida, é a folha `mulher`. O primo é a folha `primo`, sem cara, com o balão «A casa». Nas cenas quarto, fiado e primo, um bloco CENSURADO tapa-lhe o tronco. Não se gera pele nem se carrega um recorte falhado.

O tasco, por dentro, é `art/casa/tasca.jpg`: balcão, garrafas, chão de tábua, porta para a rua. O copo está no balcão, à direita, e enche-se com espaço ou com o clique enquanto se está no chão à frente do balcão. A fala do cliente fica no chão vazio à esquerda dele. O «Agora.» fica ao lado da faixa verde.

## Publicidade dentro do mundo

Dois papéis, julgados pelo JEV (`jev-1.13.0`: os dois sítios, clique em separador, papel vazio com a piada, noul 0.83). Não reabrir.

- `ads.parede`: cartaz na parede do balcão, debaixo do quadro, longe do copo.
- `ads.rua`: placard no passeio, em frente à garagem, fora das portas.

Moldura de madeira, papel creme, pregos. A imagem do patrocínio recorta-se dentro do papel. Sem imagem, lê-se «ALUGA-SE / este papel paga a casa». O clique não enche o copo nem muda o passo. Não há iframe, nem faixa no HUD, nem pausa.

Uma bifurcação do estilo, ou um terceiro sítio para dinheiro no ecrã, passa primeiro por [tasca-jev](../tasca-jev/SKILL.md).
