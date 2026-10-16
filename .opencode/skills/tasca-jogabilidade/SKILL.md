---
name: tasca-jogabilidade
description: >-
  Guarda o verbo da Tasca do Abílio: encher o copo, a rua, a fratura, a conversa,
  a tabernice que agarra, e a casa rosa onde o Zé gasta e o Matos aponta. Usar ao mudar index.html,
  o copo, a fila, a rua, o Disco, a paciência, o taberneiro, ou o ritmo da noite.
---

# Jogabilidade — Tasca do Abílio

O ficheiro é `index.html`. Canvas lógico 960×540, desenhado a 2×. Sem bibliotecas. O raycaster está em `legado.html` e não volta.

## O verbo

A noite anda-se de cima, das 22:00 às 06:00. Setas ou WASD, ou um clique no chão. Ao andar, o Zé arrota e peida. Quem está perto fala: frase curta, escolhas numeradas, um risco de tempo. Se o tempo acaba, segue quem não escolheu.

O copo fica dentro da Tasca do Abílio. Segurar (espaço ou o copo) enche. Soltar na faixa verde paga: o centro, ±0.045, paga 12 €; perto, ±0.1, paga 6 €. Um toque abaixo de 0.12 s não conta. O cliente espera cerca de 16 s.

Três fins: Apanhado, Espancado, Amanheceu. Os pontos dão o título da noite. A dívida continua no cartão, capítulos 280, 420 e 680. O HUD é bolso, hora e pontos.

A casa rosa custa 15 €. Lá dentro anda-se, como na rua: a mulher passeia, o primo entra a andar. O corpo, nas cenas do quarto, do fiado e do primo, fica tapado por um bloco «CENSURADO». «Pago no fim» chama o primo e a noite acaba no chão. «Seguir», ou sair pela porta antes de escolher, deixa voltar. Não se desenha nudez.

`document.hidden` congela o passo. O único intervalo é o cartão da noite.

## O que ainda vale

A noite de 90 s, o copo como único verbo, e o despir por tempo ficam substituídos pela noite de cima. Continuam a bolsa, o tecto, a faca e os recados.

- Recados: a faixa da Albertina ao Hilário (45 €), o santo do Padre ao Cabo (30 €), o presunto do Zeca ao Manel (40 €).
- A faca, 8 € ao António. O Cabo, com a faca no bolso, leva-a e 20 €. Sem carteira, a noite acaba na Jénierre.
- O ladrão aparece uma vez, numa zona da rua. A faca trava-o.
- O que não há na bolsa vai ao livro. O tecto é o dobro do capítulo. Passá-lo acaba a noite: o Matos leva o bolso e a faca, a dívida volta ao princípio do capítulo. A segunda vez fecha a tasca. A boca suja é só nessa cobrança.
- O primeiro minuto é uma frase, sem painel: o que se deve, e que o verde paga. O Matos diz os euros ao abrir.

## Provas

Antes de dar uma mudança de jogo por feita, jogar o fluxo no browser. Em testes, `window.TASCA_NOSAVE = true` antes de qualquer `save`. Não chamar `startNight()` num teste. Não escrever `tasca-noite-v1` nem ler ou apagar `tasca-do-ze-marosca-v1`.

Uma bifurcação do verbo, do relógio, ou de onde o dinheiro se senta passa primeiro por [tasca-jev](../tasca-jev/SKILL.md).
