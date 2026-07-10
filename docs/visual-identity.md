# Identidade visual

Este documento define a base visual do perfil de Leonardo Schmitt e do universo QA Orbit. Ele deve orientar todos os componentes futuros sem transformar o README em uma coleção de efeitos independentes.

## Princípios

- **Produto em primeiro lugar:** o QA Orbit é o centro da narrativa e da composição visual.
- **Clareza antes do efeito:** movimento, brilho e decoração nunca competem com o conteúdo.
- **Sistema, não ornamento:** cores, espaçamentos e componentes seguem regras reutilizáveis.
- **Tecnologia com personalidade:** a estética remete a dashboards, SaaS e interfaces de IA sem copiar produtos existentes.
- **Acessibilidade por padrão:** contraste, legibilidade e alternativas estáticas fazem parte da implementação.

## Paleta de cores

| Token | Cor | Uso principal |
| --- | --- | --- |
| `orbit-bg` | `#050816` | Fundo profundo e áreas externas |
| `orbit-surface` | `#0B1226` | Superfícies e cards |
| `orbit-surface-raised` | `#111C38` | Cards elevados e estados de destaque |
| `orbit-cyan` | `#22D3EE` | Ações, sinais e foco principal |
| `orbit-blue` | `#3B82F6` | Estrutura, links e informação |
| `orbit-violet` | `#6D5DFB` | IA, inovação e origem do gradiente oficial |
| `orbit-text` | `#F8FAFC` | Texto principal e marca monocromática clara |
| `orbit-muted` | `#94A3B8` | Texto secundário e metadados |
| `orbit-border` | `#233455` | Bordas e divisores |
| `orbit-success` | `#2DD4BF` | Estados saudáveis ou concluídos |
| `orbit-warning` | `#FBBF24` | Atenção e estados intermediários |

### Aplicação

- O fundo escuro e o texto claro formam a base.
- Ciano identifica o QA Orbit e as ações prioritárias.
- Azul organiza informações técnicas.
- Violeta destaca recursos relacionados a IA e inovação.
- Gradientes podem combinar ciano, azul e violeta, com baixa saturação nas áreas grandes.
- Cores de estado não devem ser usadas apenas como decoração.
- A paleta canônica e suas combinações estão definidas em `docs/qa-orbit-brand-guide.md`.

## Marca QA Orbit

- O símbolo oficial é o monograma QA integrado a uma órbita fina e um signal node.
- A versão principal usa gradiente violeta, azul e mint, sem glow.
- Glow é exclusivo de peças promocionais.
- O favicon possui geometria simplificada e não deve ser substituído pelo símbolo completo reduzido.
- Os arquivos de `assets/brand/qa-orbit/svg/` são a fonte oficial; não reconstruir a marca a partir de imagens raster.
- Regras completas de versão, redução, contraste e área de proteção estão no Brand Guide.

## Tipografia

Como o GitHub controla a renderização do Markdown, o texto nativo deve usar a pilha tipográfica da plataforma. Tipografias especiais ficam restritas a assets visuais, sempre com fallback ou conversão segura quando necessário.

- **Interface e corpo:** família sans-serif de sistema, priorizando legibilidade.
- **Títulos em assets:** `Inter`, `Space Grotesk` ou equivalente sans-serif geométrica.
- **Telemetria e metadados:** `JetBrains Mono`, `IBM Plex Mono` ou equivalente monoespaçada.
- **Pesos:** 600–700 para títulos, 500–600 para labels e 400–500 para corpo.
- **Caixa alta:** apenas em labels curtas, status e microtítulos; nunca em parágrafos.

Assets que dependam de fontes externas devem ser exportados de forma previsível e não depender do carregamento remoto para comunicar informação essencial.

## Sistema de espaçamento

A escala base é de 4 px:

| Token | Valor | Uso |
| --- | --- | --- |
| `space-1` | 4 px | Ajustes mínimos |
| `space-2` | 8 px | Elementos relacionados |
| `space-3` | 12 px | Conteúdo compacto |
| `space-4` | 16 px | Padding padrão |
| `space-6` | 24 px | Grupos internos |
| `space-8` | 32 px | Blocos e cards |
| `space-12` | 48 px | Separação entre subseções |
| `space-16` | 64 px | Separação entre seções principais |

Em telas estreitas, os espaços maiores podem ser reduzidos em um nível da escala. O ritmo vertical deve continuar perceptível mesmo quando imagens forem redimensionadas pelo GitHub.

## Títulos

- Cada seção possui um único título principal, curto e orientado à narrativa.
- Títulos usam alto contraste e peso forte.
- Um microtítulo monoespaçado pode anteceder o título para indicar módulo ou status.
- Gradientes são reservados a palavras-chave, nunca ao título inteiro por padrão.
- Linhas, números de módulo ou sinais orbitais podem acompanhar títulos, desde que sejam discretos.
- A hierarquia semântica do Markdown deve ser preservada independentemente da composição visual.

## Cards

- Fundo `orbit-surface` ou `orbit-surface-raised`.
- Borda de 1 px em `orbit-border`.
- Raio visual entre 12 e 16 px.
- Padding preferencial de 24 px.
- Sombras profundas e discretas; brilho apenas no elemento em foco.
- Cabeçalho com label, título e status opcional.
- Conteúdo curto, escaneável e com uma ação principal no máximo.
- Cards relacionados compartilham altura, alinhamento e densidade visual.

No README, cards podem ser compostos como imagens ou tabelas de apresentação apenas quando isso não prejudicar leitura, responsividade ou acessibilidade.

## SVGs

- ViewBox responsivo e dimensões previsíveis.
- Fundo compatível com a paleta escura ou transparente quando apropriado.
- Grid, órbitas e linhas técnicas usam baixa opacidade.
- Traços principais entre 1 e 2 px em escala de design.
- Gradientes têm poucos pontos de cor e contraste controlado.
- IDs internos devem possuir prefixos por componente para evitar colisões.
- Elementos decorativos devem ser separados dos elementos informativos.
- Todo SVG informativo terá texto alternativo no README e uma representação compreensível sem movimento.
- SVGs finais serão otimizados sem remover metadados necessários à acessibilidade.

## Animações

- Movimento lento e contínuo, inspirado em órbitas, pulsos e telemetria.
- Uma animação dominante por área visual; movimentos secundários devem ser sutis.
- Loops não devem apresentar cortes perceptíveis.
- Nada deve piscar rapidamente ou depender de movimento para ser entendido.
- Duração recomendada: 6–16 segundos para loops ambientais e 3–8 segundos para demonstrações funcionais curtas.
- Cada animação terá fallback estático.
- O tamanho do arquivo e o tempo de carregamento serão considerados critérios de aceite.
- Reutilização ocorrerá por padrões de movimento e arquivos-fonte, não pela duplicação de arquivos exportados.

## Responsividade e acessibilidade

- A composição parte da largura móvel e escala para desktop.
- Texto incorporado em imagens deve permanecer legível em aproximadamente 320 px de largura.
- Informação essencial também deve existir como texto no README quando necessário.
- O contraste deve atender, sempre que aplicável, ao nível AA.
- Cor, brilho e posição não podem ser os únicos indicadores de estado.
- Assets animados devem possuir uma alternativa estática equivalente.

## Restrições desta sprint

Esta sprint define apenas as regras. Nenhum SVG, GIF, ícone, badge ou animação foi produzido.
