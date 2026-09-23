# 🇧🇷 Hue

Hue melhora a comunicação de modelos de IA em português do Brasil. A skill revisa e reescreve textos para deixá-los claros, naturais e brasileiros, além de organizar respostas para facilitar a leitura e a execução.

O nome vem da expressão brasileira "hue hue hue".

## Instalação como skill

Instale com o [skills.sh](https://skills.sh/):

```bash
npx skills add getkoi/hue --skill hue
```

## Uso

Invoque a skill explicitamente:

- `/hue` em agentes compatíveis
- `$hue` no Codex

Exemplo:

```text
/hue Reescreva este texto em português do Brasil, com um tom mais natural.
```

## Plugin para ChatGPT e Codex

Este repositório também é um Agent Plugin portátil. O `plugin.json` na raiz é o manifesto principal; `.codex-plugin/plugin.json` mantém compatibilidade com clientes Codex que ainda usam esse formato.

O pacote é somente de skill: não precisa de servidor MCP, autenticação nem serviço externo. Depois de publicado no diretório universal de plugins da OpenAI, a mesma versão fica disponível nas superfícies compatíveis do ChatGPT e do Codex.

## Plugin para Claude Code

Depois que o repositório com os manifestos for publicado, adicione o marketplace e instale o plugin no Claude Code:

```text
/plugin marketplace add getkoi/hue
/plugin install hue@hue
```

Invoque a skill pelo nome qualificado do plugin:

```text
/hue:hue Reescreva este texto em português do Brasil, com um tom mais natural.
```

## O que a Hue faz

- Remove padrões comuns de texto gerado por IA.
- Corrige construções traduzidas literalmente do inglês.
- Preserva o sentido, a cobertura e a voz do autor.
- Simplifica linguagem técnica com frases curtas e termos explicados.
- Prioriza diagramas quando facilitam a explicação.
- Revisa o tamanho do texto e corta excessos sem perder entendimento.
- Adapta vocabulário, ortografia e formatação ao português brasileiro.
- Organiza respostas com informação principal primeiro, passos claros e progresso visível.

## Estrutura

- [`plugin.json`](./plugin.json): manifesto portátil para ChatGPT e Codex.
- [`.codex-plugin/plugin.json`](./.codex-plugin/plugin.json): manifesto de compatibilidade do Codex.
- [`.claude-plugin/plugin.json`](./.claude-plugin/plugin.json): manifesto nativo do Claude Code.
- [`.claude-plugin/marketplace.json`](./.claude-plugin/marketplace.json): catálogo instalável pelo Claude Code.
- [`skills/hue/SKILL.md`](./skills/hue/SKILL.md): instruções principais e checklist.
- [`skills/hue/references/padroes.md`](./skills/hue/references/padroes.md): catálogo detalhado de padrões com exemplos.
- [`skills/hue/references/exemplo.md`](./skills/hue/references/exemplo.md): calibração de voz e exemplo completo.
- [`skills/hue/references/linguagem-simples.md`](./skills/hue/references/linguagem-simples.md): exemplos de simplificação técnica, diagramas e cortes.
- [`skills/hue/agents/openai.yaml`](./skills/hue/agents/openai.yaml): apresentação e política de invocação explícita.

## Licença

[MIT](./LICENSE)
