# 🇧🇷 Hue

Hue melhora a comunicação de modelos de IA em português do Brasil. A skill revisa e reescreve textos para deixá-los claros, naturais e brasileiros, além de organizar respostas para facilitar a leitura e a execução.

O nome vem da expressão brasileira "hue hue hue".

## Instalação

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

## O que a Hue faz

- Remove padrões comuns de texto gerado por IA.
- Corrige construções traduzidas literalmente do inglês.
- Preserva o sentido, a cobertura e a voz do autor.
- Adapta vocabulário, ortografia e formatação ao português brasileiro.
- Organiza respostas com informação principal primeiro, passos claros e progresso visível.

## Estrutura

- [`SKILL.md`](./SKILL.md): instruções principais e checklist.
- [`references/padroes.md`](./references/padroes.md): catálogo detalhado de padrões com exemplos.
- [`references/exemplo.md`](./references/exemplo.md): calibração de voz e exemplo completo.
- [`agents/openai.yaml`](./agents/openai.yaml): política de invocação explícita no Codex.

## Licença

[MIT](./LICENSE)
