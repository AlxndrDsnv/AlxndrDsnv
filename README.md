<h1 align="center">Hey 👋What's Up?</h1>

###

<div align="center">
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/csharp/csharp-original.svg" height="60" alt="csharp logo"  />
  <img width="12" />
  <img src="https://skillicons.dev/icons?i=py" height="60" alt="python logo"  />
  <img width="12" />
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/javascript/javascript-original.svg" height="60" alt="javascript logo"  />
  <img width="12" />
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/css3/css3-original.svg" height="60" alt="css logo"  />
</div>

###

<div align="center">
  <img src="https://img.shields.io/static/v1?message=LinkedIn&logo=linkedin&label=&color=0077B5&logoColor=white&labelColor=&style=for-the-badge" height="25" alt="linkedin logo"  />
</div>

###

<picture>
  <source media="(prefers-color-scheme: dark)" srcset="https://raw.githubusercontent.com/AlxndrDsnv/AlxndrDsnv/pacman-output/bomberman-contribution-graph-dark.svg">
  <source media="(prefers-color-scheme: light)" srcset="https://raw.githubusercontent.com/AlxndrDsnv/AlxndrDsnv/pacman-output/bomberman-contribution-graph.svg">
  <img alt="pacman contribution graph" src="https://raw.githubusercontent.com/AlxndrDsnv/AlxndrDsnv/pacman-output/bomberman-contribution-graph.svg">
</picture>

###

## 🎮 Arcade Animation Workflow

Este repositório utiliza **GitHub Actions** para gerar automaticamente uma animação Bomberman baseada no seu histórico de contribuições do GitHub.

### ⚙️ Configuração do Workflow

O workflow (`arcade.yml`) está configurado para:

- **Executar automaticamente**: A cada 12 horas
- **Executar manualmente**: Quando disparado via `workflow_dispatch`
- **Executar ao fazer push**: Para a branch `main`

### 🔧 Como Funciona

1. **Geração do gráfico**: Utiliza a ação [`abozanona/pacman-contribution-graph`](https://github.com/abozanona/pacman-contribution-graph) para gerar um SVG animado
2. **Jogo**: Usa o jogo "Bomberman" para visualizar suas contribuições
3. **Deploy**: O gráfico gerado é enviado para a branch `pacman-output` usando [`crazy-max/ghaction-github-pages`](https://github.com/crazy-max/ghaction-github-pages)

### 📋 Detalhes Técnicos

| Configuração | Valor |
|---|---|
| **Sistema** | ubuntu-latest |
| **Timeout** | 20 minutos |
| **Token** | GITHUB_TOKEN (automático) |
| **Branch de saída** | pacman-output |
| **Diretório de build** | dist |

### 🚀 Resultado

O gráfico gerado fica disponível em:
- 🌙 **Modo escuro**: `bomberman-contribution-graph-dark.svg`
- ☀️ **Modo claro**: `bomberman-contribution-graph.svg`

E é exibido acima como uma representação visual do seu progresso! 🎯
