## AND — Material sobre Acessibilidade e Neurodivergência

Este repositório reúne o texto base ("Initial Report") e versões segmentadas em Markdown, organizadas por assunto, sobre acessibilidade e neurodivergência.

Estrutura principal
- `Initial Report.txt` — texto original usado como fonte.
- `content/` — conjunto de arquivos Markdown organizados em subpastas (design, casos, legal, market, metrics, decision, recommendations, references, etc.).
- `docs/` — arquivos gerados para publicação (MkDocs). O arquivo `docs/index.md` existe como ponto de entrada.
- `mkdocs.yml` — configuração usada para gerar um site estático com MkDocs (tema `material`).
- `scripts/` — scripts auxiliares em Python para extrair e verificar conteúdo (`extract_sections.py`, `check_snippet.py`, `verify_contents.py`).

O conteúdo em `content/` corresponde às páginas listadas em `mkdocs.yml` e pode ser usado diretamente para renderizar um site com MkDocs.

Como usar (rápido)

- Pré-requisitos: Python 3.8+ recomendado.
- Para ativar um ambiente virtual no Windows PowerShell (caso exista `.venv`):

```powershell
& .\.venv\Scripts\Activate.ps1
```

- Instalando dependências (se desejar instalar ferramentas adicionais para editar/visualizar):

```powershell
python -m pip install --upgrade pip
pip install mkdocs-material mkdocs
```

- Visualizar localmente com MkDocs:

```powershell
mkdocs serve
```

O site será servido em http://127.0.0.1:8000 enquanto o servidor estiver ativo.

Scripts úteis

- `scripts/extract_sections.py` — utilitário para extrair seções do texto original e gerar/atualizar arquivos em `content/`.
- `scripts/check_snippet.py` — checa fragmentos ou snippets dentro do conteúdo.
- `scripts/verify_contents.py` — valida a presença de arquivos esperados e referências internas.

Contribuição

Sinta-se livre para abrir issues ou pull requests. Antes de submeter PRs grandes, abra uma issue para discutir mudanças conceituais.

Licença

Há um arquivo `LICENSE` na raiz — reveja-o e mantenha conforme necessário.

Notas finais

Se quiser que eu:
- Gere uma versão atualizada de `docs/` (site estático) a partir do conteúdo;
- Gerei um `SUMMARY.md` ou ajuste na configuração do MkDocs;
- Remova arquivos de backup (`*.bak`) ou artefatos locais;

Diga qual dessas ações prefere e eu preparo as alterações.
