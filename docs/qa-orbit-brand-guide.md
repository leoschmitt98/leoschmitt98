# QA Orbit — Brand Guide v1.0

**Status:** marca congelada (Brand Freeze).

## Conceito da marca

QA Orbit representa qualidade como um sistema contínuo: sinais de automação, inteligência e engenharia circulam por um núcleo comum, são analisados e retornam ao produto como aprendizado. A marca combina precisão técnica com movimento controlado.

A identidade deve parecer uma infraestrutura de software real, não uma ilustração espacial. Por isso, a geometria é plana, o brilho não pertence à marca principal e a órbita funciona como linha de sistema, não como anel de planeta.

## Decisões a partir da referência

A referência estabelece uma direção forte, mas apresenta limitações para uso como marca:

- o Q possui mais massa que o A;
- a órbita compete com o monograma;
- volume, sombra e glow dificultam redução;
- a esfera é grande para aplicações pequenas;
- a assinatura tem espaçamento excessivo;
- as formas possuem acabamento pictórico, difícil de reproduzir consistentemente.

A reconstrução oficial preserva o gesto reconhecível e corrige esses pontos:

- Q e A usam pesos óticos equivalentes;
- o tail do Q aponta para o centro do A e conecta as letras;
- a órbita usa traço fino com terminais arredondados;
- a esfera é um signal node de apoio;
- a versão principal não possui sombra nem filtro;
- o favicon remove a esfera e simplifica o arco;
- a marca funciona em uma única cor.

## Significado do símbolo

### Monograma QA

O Q representa qualidade como núcleo observável. Seu tail é a origem da trajetória orbital, eliminando uma peça diagonal adicional e conectando significado e construção. O A representa automação e ascensão: sua forma triangular sugere direção, construção e evolução. A base e a contraforma foram ajustadas para equilibrar seu peso ótico com o Q.

### Órbita

A órbita nasce no Q e cria uma linha de continuidade em direção ao signal node. Sua parte ascendente sugere feedback retornando ao sistema. A versão v1.0 usa uma única trajetória, sem sombra ou anel paralelo, reduzindo a linguagem espacial e tornando o gesto parte funcional do monograma.

### Signal node

A esfera pequena marca um sinal em trânsito. Não representa um planeta. Em contextos reduzidos, pode ser removida sem comprometer a identidade.

## Construção geométrica

- Canvas-base: 256 × 256 unidades.
- Q: círculo externo de 62 unidades de raio e abertura interna equivalente a 24 unidades de stroke visual.
- A: triângulo estrutural com contraforma central e peso ótico alinhado ao Q.
- Órbita/tail: curva aberta de 6 unidades que nasce no interior inferior do Q.
- Signal node: raio de 7 unidades, aproximadamente 2,7% da largura do canvas.
- O conjunto preserva área interna suficiente para continuar reconhecível sem efeitos.

As formas não devem ser reconstruídas manualmente a partir de screenshots. Os arquivos em `assets/brand/qa-orbit/svg/` são a fonte oficial.

## Versões oficiais

| Versão | Arquivo | Uso |
| --- | --- | --- |
| Símbolo principal | `symbol-gradient.svg` | Interfaces e comunicação institucional |
| Símbolo flat | `symbol-flat.svg` | Contextos sem gradiente ou com renderização limitada |
| Monocromática clara | `symbol-monochrome-light.svg` | Fundos escuros e fotografia escura |
| Monocromática escura | `symbol-monochrome-dark.svg` | Fundos claros |
| Horizontal gradient | `logo-horizontal-gradient.svg` | Header, GitHub e landing page |
| Horizontal light | `logo-horizontal-light.svg` | Fundo escuro sem uso de cor |
| Horizontal dark | `logo-horizontal-dark.svg` | Fundo claro sem uso de cor |
| Vertical gradient | `logo-vertical-gradient.svg` | Apresentações e peças centralizadas |
| Vertical light | `logo-vertical-light.svg` | Peças verticais escuras |
| Vertical dark | `logo-vertical-dark.svg` | Peças verticais claras |
| Favicon | `favicon.svg` | 16–64 px e app surfaces reduzidas |
| Promotional glow | `symbol-presentation-glow.svg` | Capas e apresentações, nunca interface principal |

O logo completo corresponde ao símbolo acompanhado do wordmark `QA ORBIT`. Os lockups horizontal e vertical já incluem essa relação.

## Paleta oficial

| Token | HEX | RGB | Função |
| --- | --- | --- | --- |
| Orbit Night | `#050816` | `5, 8, 22` | Fundo principal |
| Orbit Surface | `#0B1226` | `11, 18, 38` | Superfícies elevadas |
| Orbit Blue | `#3B82F6` | `59, 130, 246` | Engenharia e eixo do gradiente |
| Signal Cyan | `#22D3EE` | `34, 211, 238` | Ação e qualidade inteligente |
| Signal Mint | `#2DD4BF` | `45, 212, 191` | Final do gradiente e estados saudáveis |
| Intelligence Violet | `#6D5DFB` | `109, 93, 251` | IA e origem do gradiente |
| Primary White | `#F8FAFC` | `248, 250, 252` | Marca e texto sobre fundos escuros |
| Secondary Text | `#94A3B8` | `148, 163, 184` | Descritores e metadados |
| Orbit Border | `#233455` | `35, 52, 85` | Linhas e estrutura |
| Promotional Glow | `#22D3EE` a 28% | `34, 211, 238` | Glow exclusivo de peças promocionais |

### Combinações permitidas

- Gradiente violet → blue → mint sobre Orbit Night ou Orbit Surface.
- Primary White sobre Orbit Night ou Orbit Surface.
- Orbit Night sobre branco ou superfícies claras neutras.
- Signal Cyan como destaque, nunca como texto longo.
- Secondary Text apenas em tamanhos confortáveis e sobre fundos escuros.

### Contraste

- Para texto funcional, priorizar Primary White sobre Orbit Night e Orbit Night sobre branco.
- O gradiente é identidade, não substituto universal para texto.
- Em contextos pequenos ou críticos, usar versão monocromática.
- Não aplicar a versão gradient sobre fundos coloridos, imagens complexas ou baixo contraste.

## Tipografia

### Produto e landing page

- Display recomendada: Inter ou Space Grotesk.
- Interface recomendada: Inter.
- Dados e labels técnicos: JetBrains Mono.

### Fallback seguro

- Wordmark e títulos: `Inter, Segoe UI, Arial, sans-serif`.
- Descritores: `JetBrains Mono, Consolas, monospace`.

Os SVGs não carregam fontes externas. O wordmark usa `QA ORBIT` em caixa alta, peso entre 600 e 700 e tracking moderado de aproximadamente `0.04em`. O descriptor usa caixa alta, peso 600 e tracking entre `0.16em` e `0.22em`.

Em textos editoriais, o produto deve ser escrito como **QA Orbit**, em title case. Caixa alta é reservada ao wordmark e a labels de interface.

## Área de proteção

Use `x` como a espessura ótica principal do monograma.

- Símbolo isolado: área livre mínima de `1x` em todos os lados.
- Logo horizontal: `1x` acima e abaixo; `1.5x` à esquerda e à direita.
- Logo vertical: `1x` ao redor do conjunto.
- Nenhum texto, borda, ícone ou recorte pode entrar nessa área.

Na geometria-base, `x` corresponde aproximadamente a 24 unidades.

## Tamanhos mínimos

| Aplicação | Mínimo recomendado |
| --- | --- |
| Favicon simplificado | 16 px |
| Símbolo completo sem descriptor | 32 px |
| Símbolo gradient com signal node | 48 px |
| Logo horizontal | 180 px de largura |
| Logo vertical | 140 px de largura |
| Lockup com descriptor legível | 260 px de largura |

Em tamanhos abaixo de 32 px, usar `favicon.svg`. Entre 32 e 47 px, preferir versão flat ou monocromática. Não usar o lockup completo quando o descriptor ficar ilegível.

## Escolha da versão

- **Símbolo:** avatares, app shell, ícones e áreas onde o nome já aparece.
- **Logo horizontal:** headers, documentação, GitHub e landing pages.
- **Logo vertical:** apresentações, capas e composições centralizadas.
- **Favicon:** 16–64 px.
- **Sem gradiente:** impressão limitada, alto contraste e interfaces pequenas.
- **Sem esfera:** favicon, 16–31 px ou gravações físicas muito pequenas.
- **Sem glow:** todas as interfaces, documentação e uso cotidiano.
- **Com glow:** apenas hero promocional, capa ou campanha com espaço suficiente.

## Uso em fundos

### Fundos escuros

Preferir as versões gradient ou light. O fundo recomendado é Orbit Night. Manter contraste entre a esfera e o fundo por meio do pequeno outline previsto no arquivo gradient.

### Fundos claros

Preferir as versões dark. A versão gradient pode ser usada somente sobre branco ou cinza muito claro e após validação visual. Não adicionar sombra para compensar contraste insuficiente.

## Usos incorretos

- Não distorcer, inclinar ou alterar proporções.
- Não redesenhar a órbita com espessura maior.
- Não aumentar a esfera.
- Não adicionar planetas, estrelas ou partículas ao símbolo oficial.
- Não trocar a ordem do gradiente.
- Não aplicar glow na versão de interface.
- Não usar contornos no monograma.
- Não separar Q e A ou mudar sua sobreposição.
- Não posicionar texto dentro da área de proteção.
- Não usar a marca gradient sobre fundos complexos.
- Não usar `QAORBIT`, `Qa Orbit` ou `qa orbit` em texto editorial.

## Aplicações

### GitHub

Usar o logo horizontal sobre fundo escuro para identificação e o símbolo para pequenos pontos de marca. O conteúdo principal deve continuar acessível em Markdown; o logo não substitui títulos semânticos. SVGs devem ser referenciados diretamente, sem dependências externas.

### Produto QA Orbit

Usar o símbolo no app shell e o lockup horizontal em autenticação, onboarding e páginas institucionais. Estados do produto usam a paleta funcional, mas não devem recolorir o símbolo conforme status.

### Landing page

Usar o logo horizontal no header e o símbolo em composições de maior escala. O glow promocional pode aparecer uma vez na primeira dobra, com intensidade controlada.

### Favicon e app icon

Usar exclusivamente `favicon.svg` entre 16 e 64 px. A microversão possui Q e A redesenhados em uma grade de 64 unidades, não possui esfera e transforma o tail em uma trajetória de 3 unidades. Para app icon em 512 px, exportar essa mesma versão com seu fundo Orbit Night e cantos arredondados.

## Brand Freeze v1.0

A geometria foi congelada após o refinamento de tail, interseção Q–A, equilíbrio ótico e microversão. Alterações futuras devem ser motivadas por falha funcional comprovada em produção, não por preferência estética. Paleta, tipografia, proporções e sistema de versões formam a identidade oficial v1.0.

### Redes sociais

O símbolo pode aparecer em avatar. Social preview exige composição própria 1200 × 630 com título, descriptor e área segura; não deve ser criado apenas ampliando o logo vertical.

## Futuras animações

O monograma permanece imóvel. Movimento pode ocorrer somente na órbita e no signal node:

- rotação ou percurso lento entre 8 e 16 segundos;
- easing suave;
- sem pulsos rápidos;
- sem distorção das letras;
- fallback estático idêntico à marca principal;
- respeito a preferências de movimento reduzido na aplicação hospedeira.

## Integração futura com o Hero

O Hero não foi alterado nesta sprint. Na integração futura:

1. O símbolo oficial substituirá o núcleo textual genérico.
2. `QA ORBIT` e `QUALITY INTELLIGENCE SYSTEM` ficarão fora ou ao lado do símbolo, em tamanho legível.
3. A órbita existente ao redor do núcleo será simplificada para evitar duplicação com a órbita da marca.
4. O símbolo terá área de proteção e não receberá telemetria sobreposta.
5. A hierarquia continuará: Leonardo Schmitt como autor, QA Orbit como produto central.
6. O logo aparecerá apenas uma vez; módulos não repetirão o símbolo.

## Arquivos e exportação

Os arquivos vetoriais oficiais estão em `assets/brand/qa-orbit/svg/`. Instruções para exportação PNG e limitações atuais estão em `assets/brand/qa-orbit/source/README.md`.
