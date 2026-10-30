# SEB Skills

Skills do Claude para produção de material didático e rotinas da escola.

## Como instalar no Claude Code

Não precisa baixar nada. No Claude Code, rode:

```
/plugin marketplace add IEEEB/seb-skills
/plugin install humanizador-escolar@seb-skills
```

Para receber atualizações depois:

```
/plugin marketplace update seb-skills
```

## Skills disponíveis

| Skill | O que faz |
|---|---|
| `humanizador-escolar` | Reescreve textos com cara de IA em português brasileiro natural e acessível para alunos, da pré-escola ao ensino médio. Tira vícios como "Vamos embarcar nessa jornada", "desempenha um papel crucial", exclamações em excesso e "Ótima pergunta!", e ajusta vocabulário e tamanho das frases à idade da turma. |

### Exemplo de uso

> Adapta esse texto sobre o ciclo da água para o meu 3º ano, ficou com muita cara de ChatGPT: [texto]

A skill devolve o texto pronto e notas curtas para o professor (nível usado, termos explicados, o que ficou de fora e dúvidas de conteúdo).

## Estrutura do repositório

```
.claude-plugin/marketplace.json     catálogo de plugins
plugins/<plugin>/
  .claude-plugin/plugin.json        dados do plugin
  skills/<skill>/SKILL.md           a skill
evals/<skill>/                      casos de teste (claude plugin eval)
```

Para adicionar uma skill nova, crie `plugins/<nome>/` com a mesma estrutura e registre o plugin em `.claude-plugin/marketplace.json`.

## Créditos

`humanizador-escolar` é uma adaptação de [blader/humanizer](https://github.com/blader/humanizer) (licença MIT).
