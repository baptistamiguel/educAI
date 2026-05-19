# Contribuindo com o educAI

Obrigado por considerar contribuir com o **educAI**! Como o projeto está **em fase de concepção**, contribuições em documentação, validação de ideias e proposta de arquitetura são muito bem-vindas.

## 1) Como abrir issues

Abra uma issue descrevendo:

- contexto e problema;
- comportamento esperado (ou proposta);
- impacto para professores, alunos ou instituições;
- sugestões de solução (opcional).

Se possível, use títulos claros, por exemplo:

- `docs: melhorar seção de MVP`
- `idea: proposta de integração com Google Meet`
- `architecture: sugestão de fila para transcrição`

## 2) Como criar branches

Use uma branch por mudança:

```bash
git checkout -b tipo/descricao-curta
```

Padrões sugeridos:

- `docs/...`
- `feat/...`
- `fix/...`
- `chore/...`

Exemplos:

- `docs/roadmap-fase-2`
- `feat/proposta-dashboard`

## 3) Como fazer commits

Faça commits pequenos, objetivos e com contexto.

```bash
git add .
git commit -m "docs: atualizar visão geral do projeto"
```

## 4) Como abrir pull requests

Ao abrir um PR:

1. explique o objetivo da mudança;
2. descreva o que foi alterado;
3. indique se houve atualização de documentação relacionada;
4. vincule a issue correspondente (`Closes #123`, quando aplicável).

## 5) Padrão de mensagens de commit

Recomendado (estilo Conventional Commits):

- `feat:` nova funcionalidade (futura implementação)
- `fix:` correção
- `docs:` documentação
- `refactor:` refatoração sem alteração de comportamento
- `test:` testes
- `chore:` manutenção

Formato:

```txt
tipo(escopo opcional): descrição curta
```

Exemplos:

- `docs(readme): detalhar funcionalidades planejadas`
- `feat(ai): propor geração de flashcards`

## 6) Boas práticas

- Mantenha o tom técnico e objetivo.
- Evite tratar funcionalidades planejadas como já implementadas.
- Prefira mudanças pequenas e revisáveis.
- Atualize documentação relacionada ao alterar visão, roadmap ou arquitetura.
- Respeite o foco educacional do projeto.
