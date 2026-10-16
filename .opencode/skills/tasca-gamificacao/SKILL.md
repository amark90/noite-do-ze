---
name: tasca-gamificacao
description: >-
  Guarda a conta e o que agarra na Tasca do Abílio: dívida, juros, paciência,
  taberneiro, fratura, e a gente que volta. Usar ao mudar capítulos, metros,
  ranks, dificuldade, recompensas, o cartão da noite, ou o que acontece depois
  de a tasca ser tua.
---

# Gamificação — Tasca do Abílio

O que agarra é andar a noite e a faixa do copo, dentro da tasca. Um número a mais no HUD mata isso. O HUD é bolso, hora e pontos. A dívida fica no cartão. O primeiro minuto é uma frase: o que se deve, e que o verde paga. Sem painel.

Três fins: Apanhado, Espancado, Amanheceu. Os pontos só dão o título da noite (aprendiz, cara da rua, da casa, quem manda na mesa, lenda). Não substituem o livro.

## A conta

Capítulos: 280 € ao Matos, 420 € à Junta, 680 € ao primo, depois a tasca é tua e os juros acabam. Juros: 7% da dívida, mínimo 10 €, zero se `matosPago`, `quiet`, ou o capítulo não leva juros. Noite = copos + rua − juros. O cartão mostra as três parcelas.

O recado da rua paga ao voltar (`banked`), não ao falar. Presunto, queijo, caracóis, a faca, a casa e a multa saem da mesma bolsa: caixa, rua, carteira, e o que falta entra na dívida se o Matos ainda escreve. A fala diz que ele apontou. O tecto é o dobro da dívida do capítulo (depois da casa, 680 €). Passar o tecto, na compra ou nos juros da manhã, acaba a noite: bolso a zero, faca fora, dívida de volta ao princípio do capítulo. A segunda vez fecha a tasca. Com o livro fechado (`lendUntil`), o fiado novo recusa-se.

## Os metros

A noite de cima não leva humor de casa, nem tabernice, nem um nome de dificuldade no HUD. O título vem dos pontos. A dívida não se escreve ao lado da hora.

Depois do capítulo 3, a casa diz-se numa frase no cartão. Não voltar a um painel do género «Gente a meio · 3 no primo · 3 contigo».

## O que não se empilha

Não juntar no balcão a dívida, a contagem da manhã, uma série de copos e um combo. Uma fratura por noite fora do meio. Uma conversa, não um quest log. A casa rosa custa 15 € por noite, pela mesma bolsa. Os quinze são o bilhete. Ficar a ver custa a noite, porque o relógio corre. O último capítulo, 680 €, é o preço da casa. Não há segundo contador. O tecto não se escreve no HUD.

O quadro é o mesmo em todas as casas. Chave local `tasca-noite-quadro` guarda só o nome. Quem fecha a casa (capítulo 3, dívida 0) manda o nome, as noites e o bolso para o livro. O cartão pede o nome nessa noite e não deixa passar sem ele. O quadro vazio diz que o nome se escreve quando a casa for tua. Menos noites primeiro; no empate, mais euros. O mesmo nome só sobe se a corrida for melhor. Dez nomes. O nome pede-se uma vez, no cartão. O quadro abre-se no título. Não é um metro no balcão. Deitar a casa abaixo não apaga o nome.

Uma bifurcação da conta ou do que conta como vitória passa primeiro por [tasca-jev](../tasca-jev/SKILL.md).
