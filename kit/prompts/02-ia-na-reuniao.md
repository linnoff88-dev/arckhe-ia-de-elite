# Hábito 2 — A IA ouvindo a reuniêo

**Por quê:** uma reuniêo gravada e transcrita vira, em segundos, uma ata e uma lista de tarefas com dono e prazo. É o trabalho de um assistente executivo por um custo quase zero.

**Como:** grave a reuniêo (com o aviso e o consentimento de todos), transcreva (o `kit/scripts/reuniao.py` faz isso no seu computador, sem enviar o áudio para ninguém) e cole a transcriçêo com o prompt abaixo.

## Prompt (copie e cole)

```text
Você é meu assistente executivo. Abaixo está a transcriçêo de uma reuniêo.
Entregue, em português:

## Ata
- Assunto e participantes
- Decisões tomadas (uma por linha)
- Pontos em aberto

## Tarefas
Uma tabela com as colunas: Responsável | O que fazer | Prazo | Trecho da fala que originou.
Regras:
- Só tarefas que alguém assumiu ou recebeu de verdade; nêo invente.
- Se o prazo nêo foi dito, escreva "sem prazo".
- Se o responsável nêo ficou claro, escreva "a definir" e liste nos pontos em aberto.

Transcriçêo:
[cole aqui]
```
