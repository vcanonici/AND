# AND Information Hub — Repositório de Conhecimento (Inicial)

Este repositório transforma o conteúdo de `Initial Report.txt` (acessibilidade para pessoas neurodivergentes) em um repositório de conhecimento segmentado, pronto para publicação no GitHub.

O que há neste repositório

- `Initial Report.txt` — arquivo fonte completo.
- `summary.md` — resumo estruturado para leitura rápida.
- `data.json` — versão resumida e estruturada em JSON.
- `query.py` — CLI simples para consultas locais (pesquisar seções, métricas e recomendações).
- `content/` — pastas e MDs segmentados por tema/subtema (pronto para navegação tema->subtema.md).

Índice rápido dos conteúdos (em `content/`)

- market/market-size.md — magnitude do mercado neurodivergente
- design/menu-design.md — princípios de design de menu acessível
- design/typography_dyslexia.md — tipografia e dislexia
- barriers/sensory_cognitive.md — barreiras sensoriais e cognitivas
- decision/cognitive_load.md — carga cognitiva e tomada de decisão
- recommendations/recommendations.md — recomendações práticas para restaurantes/hotéis
- cases/espetinho_do_vini.md — estudo de caso (Brasil)
- cases/sarang_kitchen.md — estudo de caso (Canadá)
- cases/uk_the_gate.md — estudo de caso (Reino Unido)
- legal/brazil.md — quadro legal (Brasil)
- legal/europe.md — quadro legal (Europa)
- metrics/key_metrics.md — métricas chave
- references/references.md — referências seletivas

Como usar localmente

1. (Opcional) Crie um ambiente virtual Python e ative-o.
2. Para usar a CLI localmente (pesquisa simples):

```bash
cd '/Users/vinicius/VS_Code/AND Information Hub'
python3 query.py --help
python3 query.py --list               # lista seções disponíveis
python3 query.py --show market-size   # mostra a seção 'market-size'
python3 query.py --search "fotografias"  # pesquisa por palavra-chave
```

Publicar no GitHub — passos rápidos

1. Crie um repositório vazio no GitHub (via web) e copie a URL SSH ou HTTPS.
2. No diretório do projeto execute:

```bash
git init
git add .
git commit -m "Inicial: segmentação do Initial Report em MDs + dados estruturados"
git remote add origin <URL_DO_REPO>
git branch -M main
git push -u origin main
```

Sugestões de melhorias pós-publicação

- Gerar `SUMMARY.md` automático com lista completa de MDs (útil para GitHub Pages).
- Converter `references` para `references.json` com metadados bibliográficos.
- Melhorar `query.py` para indexar `content/` e suportar pesquisa por tags e trechos.
- Criar uma versão web simples (mkdocs ou GitHub Pages) para navegação pública.

Se quiser, eu posso:

1. Gerar automaticamente um `SUMMARY.md` com índices de todos os ficheiros em `content/` e commitar; ou
2. Fazer o commit local e (se me fornecer a URL remota) adicionar o remote e dar push ao GitHub; ou
3. Expandir `query.py` para indexar todo o `content/` e suportar busca por trechos/tags.

Indique qual opção prefere e eu executo em seguida.
