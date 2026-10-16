# Tasca do Abílio — contexto para agentes

Jogo de navegador num **único ficheiro**: `index.html` (sem bibliotecas, sem build, sem passos de instalação). `legado.html` é o arquivo da versão antiga. O papel vazio abre `aluga.html`.

- **Publicação:** GitHub Pages em https://amark90.github.io/noite-do-ze/ (repo `amark90/noite-do-ze`).
- **Guardar:** o jogo grava sozinho no browser (localStorage). Sem servidor.
- **Língua e voz:** tudo em pt-PT, tom da tasca — ver `README.md` e a skill `tasca-historia`.
- **Arte:** retratos e figuras em `cast/` e `art/`.
- **Workflows do operador:** `PROMPT_MONETIZAR.md` e `PROMPT_VERIFICAR.md` (não apagar).

## Skills (`.opencode/skills/`)

| Skill | Guarda |
|---|---|
| `tasca-historia` | a voz e a gente: o Zé, o Matos, a Jénierre, falas, capítulos, nomes |
| `tasca-jogabilidade` | o verbo: encher o copo, a faixa verde, a rua, a conversa, o ritmo da noite |
| `tasca-gamificacao` | dívida, juros, paciência, taberneiro, ranks, o depois de a tasca ser tua |
| `tasca-grafismo` | um só traço, retratos em `cast/`, balcão pintado, publicidade dentro do mundo |
| `tasca-anuncios` | o dinheiro: os dois papéis, o cartão da noite, os 2 € do Matos, o placard |
| `tasca-jev` | chamar o JEV (System One) antes de bifurcar o desenho do jogo |

## Regra de ouro

O jogo é **um ficheiro só**. Não introduzas bibliotecas, bundlers ou passos de build sem pedido explícito do operador. Antes de mudanças de desenho (verbo, conta, história, estilo, dinheiro), a `tasca-jev` manda julgar primeiro no JEV: cliente em `/Users/amark/BLACKSPEAR/core/jev/client.py` (função `system_one`; chave `TYPESAFE_API_KEY` — nunca imprimir; não editar o BLACKSPEAR a partir daqui).
