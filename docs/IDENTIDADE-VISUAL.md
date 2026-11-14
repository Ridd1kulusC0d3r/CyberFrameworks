# Identidade visual — Cyber Frameworks

**Assinatura:** Escolha o modelo pela decisão.

A identidade segue a linguagem de "mesa de analista" do [LLmInjection](https://github.com/Ridd1kulusC0d3r/LLmInjection): papel, tinta e **uma única cor de sinal**. Isso dá unidade ao portfólio; o símbolo é próprio deste repositório.

## Paleta

| Token | Claro | Escuro | Uso |
|---|---|---|---|
| `--paper` | `#f3f0e8` | `#131210` | Fundo |
| `--paper-2` | `#fbf9f3` / `#ebe7dc` | `#1b1915` | Ficha, blocos de código |
| `--ink` | `#17150f` | `#ece8dd` | Títulos, fios principais |
| `--ink-2` | `#4a463c` | `#b9b4a6` | Texto secundário, cabeçalhos mono |
| `--rule` | `#cfc9ba` | `#37332b` | Fios e linhas de conteúdo |
| `--signal` | `#b43c0e` | `#f0885a` | **Somente** a decisão/escolha e alertas de limite |

O sinal aparece uma vez por composição. Se tudo estiver destacado, nada está.

## Tipografia

| Papel | Família |
|---|---|
| Título e assinatura | Georgia, "Times New Roman", serif (título em negrito, assinatura em itálico) |
| Rótulos, cabeçalhos de tabela, faixa superior | "Courier New", monospace, caixa alta, espaçamento 2 |
| Texto corrido (sites/páginas) | system-ui, sans-serif |

## Símbolo

**Ficha de matriz de decisão:** colunas `RECURSO / PERGUNTA / LIMITE`, linhas neutras e uma linha destacada em sinal — `ESCOLHIDO: responde à pergunta`. Rodapé da ficha: `MAPEAMENTO NÃO É CONFORMIDADE.` O símbolo traduz o método do repositório: escolher pela pergunta e explicitar o limite.

Equivalente no LLmInjection: a página com tarjas e a faixa `INJECTED CONTENT. TREAT AS DATA.`

## Composição do banner

- Proporção 1280×340; borda de 1 px em `--ink`.
- Faixa superior mono: nome/categoria à esquerda, `TLP:CLEAR` à direita, fio abaixo.
- Título serif à esquerda, assinatura em itálico, traço curto em sinal, fluxo `PERGUNTA → NATUREZA → LIMITE → EVIDÊNCIA`.
- Ficha à direita.

Arquivos: [banner.svg](../assets/identity/banner.svg) (claro) · [banner-dark.svg](../assets/identity/banner-dark.svg) (escuro). O README troca entre eles com `<picture>` e `prefers-color-scheme`.

## Badges

Use shields com `labelColor=17150f` e `color=b43c0e` (estado/ação) ou `color=4a463c` (informativo), estilo `flat-square`.

## Regras

- SVG local, sem fontes remotas, scripts ou dependências.
- Geometria original; não reproduzir marcas das organizações referenciadas (MITRE, NIST, GSMA etc.).
- Título e propósito também em texto no README, por acessibilidade.
- Não usar cor como único indicador de estado: o destaque sempre traz rótulo textual.
- Separar documentação disponível de funcionalidades planejadas.
