# PROMPTS — Exemplos para o educAI

> Prompts de referência para fluxos **planejados** do sistema.

## 1) Gerar resumo da aula

```txt
Você é uma assistente pedagógica. Com base na transcrição da aula abaixo, gere:
1) resumo em até 10 linhas,
2) 5 tópicos principais,
3) 3 pontos que merecem revisão.
Use linguagem clara para alunos do ensino médio.

Transcrição:
{{TRANSCRICAO}}
```

## 2) Gerar mapa mental

```txt
A partir da transcrição, estruture um mapa mental textual com:
- tema central,
- ramificações principais,
- subtemas,
- relações entre conceitos.
Formate em lista hierárquica.

Transcrição:
{{TRANSCRICAO}}
```

## 3) Gerar atividades

```txt
Com base no conteúdo da aula, crie 1 atividade rápida de 10 minutos com:
- objetivo,
- instruções,
- critérios de avaliação,
- gabarito esperado.
Adequar ao nível: {{NIVEL_TURMA}}.

Transcrição:
{{TRANSCRICAO}}
```

## 4) Gerar perguntas

```txt
Crie 8 perguntas sobre a aula:
- 3 fáceis,
- 3 intermediárias,
- 2 avançadas.
Inclua resposta curta para cada pergunta.

Transcrição:
{{TRANSCRICAO}}
```

## 5) Explicar um conceito de forma simples

```txt
Explique o conceito "{{CONCEITO}}" em linguagem simples,
com um exemplo prático do cotidiano e uma analogia curta.
Evite jargões técnicos.
```

## 6) Criar flashcards

```txt
Gere 12 flashcards no formato:
Pergunta: ...
Resposta: ...
Priorize definições, comparações e aplicações práticas do tema.

Transcrição:
{{TRANSCRICAO}}
```

## 7) Criar plano de estudo

```txt
Monte um plano de estudo de 7 dias com base na aula,
contendo:
- objetivo diário,
- tarefa prática,
- tempo estimado,
- forma de revisão.
Considere nível {{NIVEL_TURMA}}.

Transcrição:
{{TRANSCRICAO}}
```

## 8) Responder dúvidas do professor durante a aula

```txt
Contexto: você é uma assistente em tempo real para o professor.
Responda de forma curta (máximo 4 linhas), objetiva e pedagógica.
Se a pergunta pedir simplificação, use linguagem acessível.
Se pedir atividade, entregue algo aplicável em até 5 minutos.

Pergunta do professor:
{{PERGUNTA}}

Trecho recente da transcrição:
{{TRECHO_RECENTE}}
```
