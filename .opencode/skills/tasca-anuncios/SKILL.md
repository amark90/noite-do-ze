---
name: tasca-anuncios
description: >-
  Guarda o dinheiro da Tasca do Abílio: os dois papéis dentro do mundo, o cartão
  da noite, os 2 € do Matos, e o que um portal apaga. Usar ao mexer em
  anúncios, no cartaz, no placard, no cartão, no link de pagamento, ou ao
  publicar a noite.
---

# Anúncios — Tasca do Abílio

O copo não pára. O cartão da noite é o único intervalo. Não há terceiro papel, nem faixa por cima do jogo, nem iframe.

## Duas casas

Em casa, o dinheiro é teu. `window.TASCA_HOST` leva:

- `ads.parede` e `ads.rua`: `{ image, href, title }`. Sem imagem, o papel diz «ALUGA-SE / este papel / paga a casa». O clique abre `aluga.html` noutro separador. Com imagem, abre o `href`. A noite não pára. Em `aluga.html`, o botão abre `rentUrl`. Sem esse link, o botão não finge uma compra. O preço é o do link. Pago, a imagem entra à mão em `ads` e só aparece depois de publicar.
- `supportUrl`: o botão «Cala o Matos · 2 €». A página de sucesso volta com `#matos-calado` e grava `matosPago`. Sem link, o botão não finge uma compra.

Num portal, o dinheiro é deles. Se existir `window.CrazyGames.SDK` ou `window.PokiSDK`, os links externos e os 2 € não aparecem. O papel vazio e a piada ficam. O cartão pede o anúncio do SDK (`requestAd` ou `commercialBreak` / `rewardedBreak`). Se o anúncio não entra, a noite segue. O prémio, quando o anúncio acaba, é o Matos calado na noite seguinte. Não se junta o rewarded com o midgame no mesmo botão.

Poki e CrazyGames não aceitam a publicidade da casa ao lado da deles. Não se publicam as duas ao mesmo tempo.

## O que não se abre

Não se acrescenta um terceiro sítio, uma faixa, outro preço, nem um backend de anúncio. O livro dos dez nomes é a lista de quem fechou a casa, não um papel. Uma bifurcação disso passa primeiro por [tasca-jev](../tasca-jev/SKILL.md). O desenho dos papéis está em [tasca-grafismo](../tasca-grafismo/SKILL.md). O cartão e os juros estão em [tasca-gamificacao](../tasca-gamificacao/SKILL.md).
