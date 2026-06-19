# CLAUDE.md — llm-council

## O que é este repo

Uma skill do Claude distribuída como repositório público no GitHub. A única
fonte de verdade do comportamento é `skills/llm-council/SKILL.md`. Toda mudança
de comportamento começa por lá.

A skill implementa o LLM Council de Andrej Karpathy: 5 conselheiros de IA com
lentes opostas, revisão cruzada anônima e síntese de um presidente. O repo é uma
vitrine — o README é uma landing page, não só documentação.

## O que editar

| Arquivo | O que controla |
|---------|----------------|
| `skills/llm-council/SKILL.md` | Comportamento — triggers, fluxo, formato de saída. PT-BR, canônico. |
| `skills/llm-council/references/metodo-canonico.md` | Perfil dos 5 conselheiros, presidência, template do relatório HTML. |
| `skills/llm-council/evals/evals.json` | Casos de teste de trigger e comportamento. |
| `skills/llm-council/README.md` | Resumo por-skill voltado pra humano. |
| `README.md` (raiz) | Porta de entrada do produto. Otimizar pra quem decide sob incerteza. |
| `assets/social-preview.html` | Instância do gabarito DS V3.0 (motivo council) do social card. |
| `page/index.html` | Página-vitrine interativa publicada na Vercel. |

## O que NÃO editar

- Não edite a skill canônica no monorepo privado `mscs-skills` a partir daqui —
  este repo é um espelho publicado. Mudanças de comportamento fluem pelo `skills-sync`.
- Mantenha o frontmatter do SKILL.md (`name`, `description`) intacto.
- Não fabrique números de eficácia. O valor vem do método, não de marketing.
- Nunca commite `.env`, tokens ou credenciais.

## Convenções

- Idioma: README/skill em PT-BR; voz Tradutor, frases curtas, voz ativa, zero floreio.
- Commits: Conventional Commits. Push só com SHA verificado (local = remote).

## Licença

MIT. Contribuições bem-vindas. Ver CONTRIBUTING.md.
