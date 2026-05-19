# ARCHITECTURE — Arquitetura inicial sugerida

> Esta arquitetura é **proposta** e serve como base para evolução do projeto.

## 1. Frontend

- Aplicação web (ex.: Next.js) para:
  - autenticação de usuários;
  - gestão de aulas;
  - visualização de transcrição e materiais;
  - interação com assistente de IA.

## 2. Backend

- API (ex.: Node.js/NestJS ou Python/FastAPI) para:
  - orquestrar fluxos de aula e processamento;
  - persistir dados de usuários/aulas;
  - acionar serviços de IA e transcrição;
  - disponibilizar endpoints para dashboard.

## 3. Banco de dados

- Banco relacional (ex.: PostgreSQL) para:
  - usuários e permissões;
  - metadados de aulas;
  - histórico de materiais gerados;
  - relacionamento entre turmas, disciplinas e conteúdos.

## 4. IA / transcrição

- Camada de Speech-to-Text para transcrição em tempo real/lote.
- Camada LLM para:
  - sumarização;
  - geração de perguntas/atividades;
  - explicações simplificadas;
  - criação de flashcards e plano de estudo.

## 5. Armazenamento

- Object storage (ex.: S3/GCS) para:
  - gravações de áudio (quando permitido);
  - transcrições brutas;
  - materiais exportados.

## 6. Autenticação

- Proposta inicial:
  - login por e-mail/senha;
  - suporte futuro a SSO (Google/Microsoft);
  - controle de acesso por perfil (professor, coordenação, admin).

## 7. Integrações externas

- Plataformas de videoconferência (futuro):
  - Google Meet
  - Zoom
  - Microsoft Teams
- Serviços de IA/STT (conforme estratégia de custo e qualidade).

## 8. Fluxo básico dos dados (proposto)

1. Professor inicia aula e ativa o educAI.
2. Módulo de captura envia áudio ao serviço de transcrição.
3. Transcrição é armazenada e disponibilizada em tempo real.
4. Comandos do professor acionam geração de conteúdo no módulo de IA.
5. Resultados são persistidos e exibidos no frontend.
6. Ao final da aula, o sistema gera materiais consolidados.

```txt
[Chamada online]
      |
      v
[Captura de áudio] --> [Serviço STT] --> [Transcrição]
                                  |           |
                                  v           v
                            [Módulo IA] --> [API Backend] --> [Frontend]
                                  |
                                  v
                           [Banco + Storage]
```
