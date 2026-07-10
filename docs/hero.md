# Hero — especificação do componente

## Conceito

O Hero apresenta o perfil como a interface de entrada do **QA Orbit Quality Intelligence System**. A composição une uma mensagem humana, à esquerda, a um sistema orbital técnico, à direita. Leonardo não aparece como uma lista de competências: aparece como o engenheiro construindo o sistema.

O conceito proprietário é chamado **Orbit Core**. Um núcleo central recebe e distribui sinais entre três disciplinas que formam o trabalho de Leonardo:

- **Automation:** módulo ciano, representado por dois chevrons de execução. Comunica fluxo, repetibilidade e feedback contínuo.
- **Artificial Intelligence:** módulo violeta, representado por uma rede neural mínima de quatro nós. Comunica inferência e conexão.
- **Software Engineering:** módulo azul, representado por brackets de código. Comunica estrutura e construção.

Os três módulos compartilham a mesma geometria de cápsula, contorno técnico e conexão orbital. A diferença está no glifo e na cor funcional, mantendo todos como partes do mesmo produto.

## Layout

O canvas possui duas zonas, sem divisor rígido:

- **Narrativa — 48%:** ocupa `x=72–555`. Contém eyebrow, nome, slogan, manifesto e CTA.
- **Sistema — 52%:** ocupa `x=570–1200`. Contém núcleo, órbitas, módulos e telemetria.

Uma linha de sinal conecta visualmente o CTA ao sistema, formando um percurso da proposta para o produto. O fundo usa grid de 32 px com máscara de opacidade, além de dois campos luminosos muito suaves.

## Conteúdo

| Elemento | Texto |
| --- | --- |
| Eyebrow | `QA ENGINEER · FULL-STACK BUILDER` |
| Título | `LEONARDO SCHMITT` |
| Slogan | `Engineering quality beyond testing.` |
| Manifesto | `I build intelligent systems where automation, AI,`<br>`and software engineering converge.` |
| CTA | `EXPLORE QA ORBIT` |
| Produto | `QA ORBIT` |
| Descriptor | `QUALITY INTELLIGENCE SYSTEM` |

O CTA será visual nesta sprint. Quando o Hero for integrado ao README, a imagem poderá ser envolvida por um link para o repositório ou produto QA Orbit sem alterar o SVG.

## Dimensões e grid

- **Largura:** 1200 px.
- **Altura:** 560 px.
- **ViewBox:** `0 0 1200 560`.
- **Grid estrutural:** 12 colunas de 76 px.
- **Gutters:** 20 px.
- **Margens externas:** 32 px para a moldura e 72 px para conteúdo.
- **Grid de fundo:** módulos de 32 px.
- **Raio da moldura:** 24 px.
- **Área segura:** 40 px em todos os lados.
- **Centro orbital:** `(888, 280)`.
- **Órbita interna:** 128 × 92 px.
- **Órbita intermediária:** 220 × 154 px.
- **Órbita externa:** 304 × 220 px.

## Hierarquia visual

1. Nome de Leonardo, em branco azulado e 54 px.
2. Núcleo QA Orbit, com maior contraste da zona direita.
3. Slogan, em 27 px, com destaque ciano em `quality`.
4. Módulos orbitais, com labels monoespaçados.
5. Manifesto e CTA.
6. Grid, coordenadas e microtelemetria em baixa opacidade.

## Tipografia

O SVG usa apenas fallbacks locais para não depender de rede:

- **Display:** `Inter, Segoe UI, Arial, sans-serif`.
- **Técnica:** `JetBrains Mono, Consolas, monospace`.
- **Nome:** 54 px, peso 700, tracking de -1.5 px.
- **Slogan:** 27 px, peso 500.
- **Manifesto:** 16 px, peso 400, line-height visual de 26 px.
- **Eyebrow e telemetria:** 11–12 px, peso 600, tracking de 1.6–2.4 px.
- **Núcleo:** 22 px, peso 700.

## Cores

| Papel | Valor |
| --- | --- |
| Fundo | `#050816` |
| Superfície | `#0B1226` |
| Superfície elevada | `#111C38` |
| Texto | `#E6F1FF` |
| Texto secundário | `#94A3B8` |
| Borda | `#233455` |
| Ciano / QA Orbit / Automation | `#22D3EE` |
| Azul / Engineering | `#3B82F6` |
| Violeta / AI | `#8B5CF6` |
| Sinal positivo | `#2DD4BF` |

O brilho é obtido somente com gradientes transparentes e filtros suaves. Nenhuma área usa neon sólido em grande escala.

## Elementos do sistema

### Núcleo QA Orbit

Um círculo técnico de 112 px contém um monograma `QO`, o nome do produto e seu descriptor. Três pequenos pontos internos representam sinais de qualidade sendo analisados. Anéis concêntricos reforçam a ideia de plataforma central.

### Órbitas

Três elipses com inclinações distintas criam profundidade sem simular 3D. Partes pontilhadas indicam trânsito de dados; arcos sólidos estabelecem a estrutura.

### Módulos

Cada módulo combina um nó circular com um glifo proprietário e um label. As posições formam um triângulo ao redor do núcleo:

- Automation: superior direita.
- AI: inferior direita.
- Engineering: esquerda inferior.

### Linhas técnicas e telemetria

Conectores de 1 px saem do sistema para labels técnicos curtos. Coordenadas, ticks e barras de sinal criam contexto de interface, mas usam opacidade baixa para não disputar atenção.

## Desktop

Entre 768 e 1200 px de largura renderizada, o SVG preserva a composição em duas zonas. O sistema orbital permanece dominante, mas o nome é o primeiro ponto de leitura. A proporção fixa evita reflow inesperado no GitHub.

## Mobile

Entre 320 e 767 px, o mesmo SVG é reduzido proporcionalmente. Para manter legibilidade:

- o nome e o núcleo usam tamanhos de origem grandes;
- o manifesto possui apenas duas linhas;
- detalhes secundários usam contraste baixo e podem se tornar textura visual sem comprometer a mensagem;
- nenhum texto essencial está nas microtelemetrias;
- a composição mantém área segura e não depende de elementos nas bordas.

Na integração futura, o texto essencial também existirá em Markdown acessível. Se testes reais indicarem leitura insuficiente abaixo de 360 px, será criada uma variante `hero-mobile.svg` na sprint de integração, sem alterar a identidade definida aqui.

## Critérios de aceite

- Asset vetorial original e autocontido.
- Nenhuma imagem externa, JavaScript ou animação.
- Leitura clara em fundo claro ou escuro do GitHub graças à moldura própria.
- IDs internos prefixados com `hero-`.
- Título e descrição acessíveis dentro do SVG.
- Elementos decorativos agrupados separadamente.
- Nenhum componente fora do Hero implementado.

## Refinamento de legibilidade e movimento

O Hero possui duas variantes derivadas da mesma geometria:

- `assets/svg/hero/hero-static.svg`: versão estática e fallback publicado no README.
- `assets/svg/hero/hero-animated.svg`: versão com movimento sutil para validação no GitHub.

### Ajustes tipográficos

- Nome: 54 → 60 px, peso 700 → 750 e tracking menos negativo.
- Slogan: 27 → 30 px, peso 500 → 600 e branco de maior contraste.
- Apoio: 16 → 18 px, peso 400 → 500, line-height visual de 29 px.
- CTA: 11 → 13 px, fonte sans-serif e área de 220 × 48 px.
- QA Orbit: 22 → 25 px.
- Labels Automation, Engineering e AI: 8,5 → 10,5/11 px com fonte sans-serif.
- Coordenadas, sinal numérico e metadata de build foram removidos por não agregarem significado.

### Movimento

- Órbita externa: rotação linear de 40 segundos.
- Órbita interna: rotação inversa de 28 segundos.
- Núcleo: pulso entre 98,5% e 101,8% em 5 segundos.
- Signal nodes: pulsos alternados de opacidade em 4,8 segundos.
- Telemetria: deslocamento lento de dash em 12 segundos.
- Módulos: flutuação independente entre 1,5 e 2 px, sem movimentar os grupos de texto separadamente.
- Grid, copy e CTA permanecem estáticos.

`prefers-reduced-motion: reduce` desativa todas as animações e preserva a composição completa.

### Estratégia de publicação

O README permanece referenciando `hero-static.svg` até que `hero-animated.svg` seja publicado e observado no renderer real do GitHub. A versão animada não deve substituir o fallback apenas com base no teste local.
