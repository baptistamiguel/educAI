# educAI

![Status](https://img.shields.io/badge/status-Em%20fase%20de%20concep%C3%A7%C3%A3o-orange)
![Licença](https://img.shields.io/badge/licen%C3%A7a-MIT-blue)

**educAI** é uma ideia de plataforma para apoiar aulas online com IA em tempo real: transcrição automática, apoio durante a chamada e geração de materiais pedagógicos ao final.

## Status do projeto

**Em fase de concepção**.

## Visão geral

O educAI propõe uma experiência inspirada em assistentes de reunião, mas direcionada ao contexto educacional. A IA participa da aula, transcreve o conteúdo em tempo real e ajuda o professor a transformar a aula em recursos práticos de estudo.

## Problema

Professores e instituições frequentemente enfrentam:

- dificuldade em registrar e organizar o conteúdo de aulas ao vivo;
- tempo elevado para transformar aulas em materiais de revisão;
- pouca visibilidade sobre os principais pontos e dúvidas recorrentes.

## Solução proposta

Uma plataforma onde a IA:

1. entra na aula/chamada online;
2. escuta e transcreve a conversa em tempo real;
3. atua como assistente durante a aula (sob demanda do professor);
4. gera materiais educacionais estruturados ao final.

## Funcionalidades principais (planejadas)

| Categoria | Funcionalidade | Estado |
| --- | --- | --- |
| Transcrição | Captura e transcrição de áudio em tempo real | Planejado |
| Assistente ao vivo | Resumo instantâneo, simplificação de conceito, perguntas rápidas | Planejado |
| Pós-aula | Resumo, tópicos principais e destaques | Planejado |
| Conteúdo educacional | Atividades, perguntas, flashcards e plano de estudo | Planejado |
| Organização | Marcação de trechos importantes durante a aula | Planejado |

## Público-alvo

- Professores do ensino básico, técnico e superior
- Criadores de cursos e professores particulares
- Coordenações pedagógicas e instituições de ensino
- Alunos que precisam de materiais de revisão estruturados

## Exemplo de uso

1. Professor inicia uma aula no Google Meet/Zoom/Teams (integração futura).
2. O bot do educAI participa da chamada e inicia a transcrição.
3. Durante a aula, o professor pergunta: *"Explique esse conceito de forma mais simples"*.
4. O sistema responde em tempo real com uma explicação simplificada.
5. Ao final, o professor gera:
   - resumo da aula;
   - tópicos principais;
   - atividade rápida;
   - flashcards;
   - plano de estudo.

## Possíveis telas do sistema (propostas)

- Tela de login/cadastro
- Dashboard de aulas
- Tela de aula em andamento (transcrição ao vivo + assistente)
- Tela de materiais gerados
- Biblioteca/histórico de aulas
- Tela de configurações (turmas, idioma, preferências de geração)

## Tecnologias sugeridas

| Camada | Opções sugeridas |
| --- | --- |
| Frontend | React + Next.js |
| Backend | Node.js (NestJS/Express) ou Python (FastAPI) |
| Banco de dados | PostgreSQL |
| IA/LLM | OpenAI, Anthropic ou modelos open-source |
| STT (Speech-to-Text) | Whisper, Deepgram, Google Speech-to-Text |
| Infra | Docker + cloud (AWS/GCP/Azure) |

## Arquitetura inicial (proposta)

- **Frontend web** para professores e gestão de aulas.
- **API backend** para autenticação, orquestração e geração de conteúdo.
- **Módulo de transcrição em tempo real** para captura e processamento do áudio.
- **Pipeline de IA** para sumarização e geração de materiais.
- **Armazenamento** de transcrições, arquivos e materiais gerados.

> Veja mais em [`docs/ARCHITECTURE.md`](/docs/ARCHITECTURE.md).

## MVP (escopo inicial)

- Upload de áudio ou gravação de aula
- Transcrição automática
- Geração de resumo e tópicos principais
- Geração de perguntas e atividade simples
- Histórico básico de aulas

## Roadmap

O roadmap completo está em [`ROADMAP.md`](/ROADMAP.md).

Resumo das fases:

1. MVP de transcrição + resumo
2. Melhorias de IA educacional
3. Integrações com Meet, Zoom e Teams
4. Dashboard educacional
5. Recursos avançados para escolas

## Diferenciais

- Foco em educação (não apenas reuniões genéricas)
- Assistência pedagógica em tempo real durante a aula
- Conversão direta de aula em materiais de estudo
- Potencial de padronização de apoio didático para turmas

## Benefícios

### Para professores

- Redução do tempo de preparação pós-aula
- Apoio em tempo real para dinâmicas de ensino
- Registro estruturado do conteúdo ministrado

### Para alunos

- Acesso a resumos e revisões mais claras
- Materiais personalizados para estudo
- Maior retenção de conteúdo

### Para instituições

- Melhor organização pedagógica
- Base de conhecimento de aulas e conteúdos
- Potencial de melhoria de desempenho acadêmico

## Como rodar o projeto futuramente

Como o projeto está em fase de concepção, ainda não há aplicação executável. Uma proposta de fluxo futuro:

```bash
# 1) Clonar o repositório
git clone https://github.com/<usuario>/educAI.git

# 2) Entrar no diretório
cd educAI

# 3) Instalar dependências (exemplo Node.js)
npm install

# 4) Configurar variáveis de ambiente
cp .env.example .env

# 5) Iniciar ambiente de desenvolvimento
npm run dev
```

> Esses comandos são **propostos** e serão ajustados quando houver implementação.

## Estrutura sugerida de pastas

```txt
educAI/
├── docs/
│   ├── IDEA.md
│   ├── FEATURES.md
│   ├── ARCHITECTURE.md
│   └── PROMPTS.md
├── frontend/              # futuro
├── backend/               # futuro
├── services/
│   ├── transcription/     # futuro
│   └── ai-generation/     # futuro
├── infra/                 # futuro
├── README.md
├── CONTRIBUTING.md
├── ROADMAP.md
└── LICENSE
```

## Conclusão

O **educAI** nasce como uma proposta para tornar aulas online mais produtivas, com IA como suporte pedagógico antes, durante e depois da aula. Neste momento, o repositório documenta a visão, o escopo e os próximos passos de implementação.
