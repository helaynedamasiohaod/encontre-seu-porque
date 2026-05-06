# MEMORY — Encontre seu Porquê

Registro do que foi construído, decisões tomadas e contexto do projeto.

---

## Contexto

Projeto criado para o **clube do livro** da Helayne, que está lendo *Encontre seu Porquê* de Simon Sinek.

O objetivo foi transformar o método do livro em ferramentas conversacionais práticas — para que cada membro do clube possa vivenciar a descoberta do próprio Porquê através de uma conversa guiada com IA.

**Repositório:** https://github.com/helaynedamasiohaod/encontre-seu-porque
**Conta GitHub:** helaynedamasiohaod (pública)

---

## O que foi criado

### Versão 1 — Claude Code

| Item | Detalhe |
|------|---------|
| Formato | Skill AIOX (`.zip`) |
| Comando de ativação | `/encontre-seu-porque` |
| Instalação | `/skill install encontre-seu-porque-claude.zip` |
| Diretório | `encontre-seu-porque-claude/` |
| Arquivos | `SKILL.md` + `references/sinek-method.md` |
| Criado com | `skill-creator` (init + package) |

**Prompt:** parceiro conversacional em 5 fases progressivas. Formato de frase de propósito: *"Acredito que... Por isso ajudo..."*

### Versão 2 — ChatGPT

| Item | Detalhe |
|------|---------|
| Formato | Prompt `.md` para copiar e colar |
| Funciona em | Qualquer plano ChatGPT (inclusive gratuito) |
| Diretório | `encontre-seu-porque-chatgpt/` |
| Arquivo | `prompt.md` |

**Prompt:** versão diferente da v1 — inclui seção de "Erros Críticos", Método 2 de estímulo de memória, proibição explícita de perguntas "Por que?", e formato de frase *"..., de modo que..."* (Sinek, Mead e Docker).

---

## Estrutura do repositório

```
encontre-seu-porque/
├── encontre-seu-porque-claude/
│   ├── SKILL.md
│   └── references/
│       └── sinek-method.md
├── encontre-seu-porque-claude.zip
├── encontre-seu-porque-chatgpt/
│   └── prompt.md
├── README.md
├── MEMORY.md
└── .gitignore
```

---

## Decisões e o porquê de cada uma

**Skill com zip para Claude, prompt simples para ChatGPT**
O Claude Code tem sistema nativo de instalação de skills via `.zip`. O ChatGPT não tem — o único mecanismo é texto colado na conversa.

**Repositório público**
Para facilitar o compartilhamento com o clube sem precisar convidar cada pessoa individualmente.

**Nomes com prefixo completo**
`encontre-seu-porque-claude` e `encontre-seu-porque-chatgpt` em vez de `encontre-seu-porque/` e `chatgpt/`. Ficou mais claro e consistente visualmente.

**Link do repositório raiz para compartilhar**
Usar `https://github.com/helaynedamasiohaod/encontre-seu-porque` em vez de link direto para arquivo — evita o `/blob/main/` na URL e direciona para o README que já explica tudo.

---

## Diferenças entre as versões

| Aspecto | v1 Claude | v2 ChatGPT |
|---------|-----------|------------|
| Formato do Porquê | "Acredito que... Por isso ajudo..." | "..., de modo que..." |
| Erros críticos | Implícitos nos princípios | Seção explícita no topo |
| Estímulo de memória | Fase 2 de exploração | Método 2 dedicado |
| Pergunta "Por quê?" | Não mencionada | Explicitamente proibida |
| Autores referenciados | Sinek | Sinek, Mead e Docker |

---

## Mensagem aprovada para o grupo

> Oi pessoal! Criei uma experiência conversacional baseada no livro que estamos lendo.
>
> A ideia é simples: você tem uma conversa guiada que ajuda a descobrir o seu Porquê através das suas próprias histórias de vida. Sem respostas prontas, sem coaching — só você, suas memórias e um parceiro que faz as perguntas certas.
>
> Tem versão para **Claude Code** e para **ChatGPT** (funciona no plano gratuito).
>
> Acesse aqui e siga as instruções: https://github.com/helaynedamasiohaod/encontre-seu-porque
>
> Boa jornada! 🔍

---

## Próximos passos (em aberto)

- Versão 3 — agente AIOX ativável via `@porquê` dentro do Claude Code (Caminho 1)
- Versão 4 — squad completo com agente facilitador + extração de padrões + síntese + relatório final (Caminho 3)
