# ðŸ§  IA de Elite â€” 7 hÃ¡bitos de quem usa IA no topo

<div align="center">
  <img src="capa/logo.svg" alt="Arckhé AI" height="48" />
  <p><strong>Arckhé AI</strong></p>
</div>


**ðŸ‡§ðŸ‡· [PortuguÃªs](README.md) Â· ðŸ‡ºðŸ‡¸ [English](README.en.md) Â· ðŸ‡ªðŸ‡¸ [EspaÃ±ol](README.es.md)**

[![IA de Elite](capa/capa.png)](https://linnoff88-dev.github.io/

## O que Ã©

IA de Elite Ã© um guia com os 7 hÃ¡bitos que separam quem usa a IA de verdade de quem sÃ³ faz perguntas soltas no chat: falar em vez de digitar, deixar a IA ouvir a reuniÃ£o, pedir visual em vez de texto, ser entrevistado pela IA, pedir falhas, testar com as prÃ³prias mÃ£os e manter a mente aberta. Serve para qualquer pessoa que jÃ¡ usa ChatGPT, Claude ou Gemini. Junto vem um kit aberto e grÃ¡tis com 7 prompts para copiar, 4 skills para o Claude Code e scripts que rodam no seu computador. Para os prompts basta um chat; para os scripts, Python.

## ðŸ“– Guia de uso

Guia completo (landing + passo a passo): **https://linnoff88-dev.github.io/

## Os 7 hÃ¡bitos

| # | HÃ¡bito | No kit |
|---|---|---|
| 1 | **Fale, nÃ£o digite** â€” em mÃ©dia 30â€“50 palavras/min digitando Ã— 150â€“200 falando | `prompts/01`, `scripts/ditado.md`, `scripts/ditado.sh` |
| 2 | **A IA ouvindo a reuniÃ£o** â€” transcriÃ§Ã£o vira ata e tarefas (quem, o quÃª, prazo) | `scripts/reuniao.py`, `prompts/02` |
| 3 | **Mostre, nÃ£o conte** â€” HTML, grÃ¡ficos, 3D em vez de texto | `prompts/03`, skill `mostra-nao-conta` |
| 4 | **A IA te entrevista** â€” "me faÃ§a todas as perguntas que precisa" | `prompts/04`, skill `entrevista-me` |
| 5 | **PeÃ§a falhas, nÃ£o opiniÃ£o** â€” a IA tende a concordar; peÃ§a o que estÃ¡ errado | `prompts/05`, skill `fure-minha-ideia` |
| 6 | **Teste vocÃª mesmo** â€” peÃ§a para fazer em vez de perguntar se consegue | `prompts/06`, skill `testa-agora` |
| 7 | **Mente aberta** â€” testar Ã© barato, nÃ£o testar custa caro | `prompts/07` |

## O kit

```
kit/
â”œâ”€â”€ prompts/        7 prompts prontos (um por hÃ¡bito)
â”œâ”€â”€ skills/         entrevista-me Â· fure-minha-ideia Â· mostra-nao-conta Â· testa-agora
â”œâ”€â”€ scripts/        reuniao.py Â· ditado.sh Â· ditado.md
â”œâ”€â”€ exemplos/       reuniao-exemplo.txt Â· painel-falar-vs-digitar.html
â”œâ”€â”€ testes/rodar.sh valida o kit sem rede e sem API
â””â”€â”€ instalar.sh     copia as skills para ~/.claude/skills/
```

## ComeÃ§o rÃ¡pido

```bash
git clone https://github.com/linnoff88-dev/ia-de-elite.git && cd ia-de-elite
bash kit/testes/rodar.sh                          # 30 ok Â· 0 falha(s)
python3 kit/scripts/reuniao.py --simular --saida teste-reuniao
bash kit/instalar.sh --dry-run                    # depois sem --dry-run
```

- **reuniao.py**: Ã¡udio/vÃ­deo (ou .txt/.srt) â†’ `transcricao.txt`, `ata.md`, `tarefas.md`. Transcreve **no seu computador** com faster-whisper (`pip install faster-whisper`). A ata sai pelo `claude -p` (assinatura do Claude Code), pelo Ollama local ou como prompt para colar em qualquer chat (`--motor prompt`). Nunca chama API paga.
- **ditado.sh** (Linux): grava, transcreve local e copia o texto. Windows: `Win + H`. macOS: `Fn` duas vezes.

Aberto e grÃ¡tis Â· licenÃ§a MIT Â· [ARCKHÉ AI](https://ARCKHÉ AI)

---

<div align="center">
  <img src="capa/logo.svg" alt="Arckhé AI" height="32" />
  <p><strong>Arckhé AI</strong></p>
</div>