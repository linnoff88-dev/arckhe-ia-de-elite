# ê°Å¸Â§Â  IA de Elite ê¢â¬â 7 hêÂ¡bitos de quem usa IA no topo

<div align="center">
  <img src="capa/logo.svg" alt="Arckhé AI" height="48" />
  <p><strong>Arckhé AI</strong></p>
</div>


**ê°Å¸â¡Â§ê°Å¸â¡Â· [PortuguêÂªs](README.md) êÂ· ê°Å¸â¡Âºê°Å¸â¡Â¸ [English](README.en.md) êÂ· ê°Å¸â¡Âªê°Å¸â¡Â¸ [EspaêÂ±ol](README.es.md)**

[![IA de Elite](capa/capa.png)](https://linnoff88-dev.github.io/

## O que êÂ©

IA de Elite êÂ© um guia com os 7 hêÂ¡bitos que separam quem usa a IA de verdade de quem sêÂ³ faz perguntas soltas no chat: falar em vez de digitar, deixar a IA ouvir a reuniêÂ£o, pedir visual em vez de texto, ser entrevistado pela IA, pedir falhas, testar com as prêÂ³prias mêÂ£os e manter a mente aberta. Serve para qualquer pessoa que jêÂ¡ usa ChatGPT, Claude ou Gemini. Junto vem um kit aberto e grêÂ¡tis com 7 prompts para copiar, 4 skills para o Claude Code e scripts que rodam no seu computador. Para os prompts basta um chat; para os scripts, Python.

## ê°Å¸ââ Guia de uso

Guia completo (landing + passo a passo): **https://linnoff88-dev.github.io/

## Os 7 hêÂ¡bitos

| # | HêÂ¡bito | No kit |
|---|---|---|
| 1 | **Fale, nêÂ£o digite** ê¢â¬â em mêÂ©dia 30ê¢â¬â50 palavras/min digitando êâ 150ê¢â¬â200 falando | `prompts/01`, `scripts/ditado.md`, `scripts/ditado.sh` |
| 2 | **A IA ouvindo a reuniêÂ£o** ê¢â¬â transcriêÂ§êÂ£o vira ata e tarefas (quem, o quêÂª, prazo) | `scripts/reuniao.py`, `prompts/02` |
| 3 | **Mostre, nêÂ£o conte** ê¢â¬â HTML, grêÂ¡ficos, 3D em vez de texto | `prompts/03`, skill `mostra-nao-conta` |
| 4 | **A IA te entrevista** ê¢â¬â "me faêÂ§a todas as perguntas que precisa" | `prompts/04`, skill `entrevista-me` |
| 5 | **PeêÂ§a falhas, nêÂ£o opiniêÂ£o** ê¢â¬â a IA tende a concordar; peêÂ§a o que estêÂ¡ errado | `prompts/05`, skill `fure-minha-ideia` |
| 6 | **Teste vocêÂª mesmo** ê¢â¬â peêÂ§a para fazer em vez de perguntar se consegue | `prompts/06`, skill `testa-agora` |
| 7 | **Mente aberta** ê¢â¬â testar êÂ© barato, nêÂ£o testar custa caro | `prompts/07` |

## O kit

```
kit/
ê¢âÅê¢ââ¬ê¢ââ¬ prompts/        7 prompts prontos (um por hêÂ¡bito)
ê¢âÅê¢ââ¬ê¢ââ¬ skills/         entrevista-me êÂ· fure-minha-ideia êÂ· mostra-nao-conta êÂ· testa-agora
ê¢âÅê¢ââ¬ê¢ââ¬ scripts/        reuniao.py êÂ· ditado.sh êÂ· ditado.md
ê¢âÅê¢ââ¬ê¢ââ¬ exemplos/       reuniao-exemplo.txt êÂ· painel-falar-vs-digitar.html
ê¢âÅê¢ââ¬ê¢ââ¬ testes/rodar.sh valida o kit sem rede e sem API
ê¢ââê¢ââ¬ê¢ââ¬ instalar.sh     copia as skills para ~/.claude/skills/
```

## ComeêÂ§o rêÂ¡pido

```bash
git clone https://github.com/linnoff88-dev/ia-de-elite.git && cd ia-de-elite
bash kit/testes/rodar.sh                          # 30 ok êÂ· 0 falha(s)
python3 kit/scripts/reuniao.py --simular --saida teste-reuniao
bash kit/instalar.sh --dry-run                    # depois sem --dry-run
```

- **reuniao.py**: êÂ¡udio/vêÂ­deo (ou .txt/.srt) ê¢â â `transcricao.txt`, `ata.md`, `tarefas.md`. Transcreve **no seu computador** com faster-whisper (`pip install faster-whisper`). A ata sai pelo `claude -p` (assinatura do Claude Code), pelo Ollama local ou como prompt para colar em qualquer chat (`--motor prompt`). Nunca chama API paga.
- **ditado.sh** (Linux): grava, transcreve local e copia o texto. Windows: `Win + H`. macOS: `Fn` duas vezes.

Aberto e grêÂ¡tis êÂ· licenêÂ§a MIT êÂ· [ARCKHê AI](https://ARCKHê AI)

---

<div align="center">
  <img src="capa/logo.svg" alt="Arckhé AI" height="32" />
  <p><strong>Arckhé AI</strong></p>
</div>