# Arquitetura do projeto

## Objetivo

Este repositório trata o GitHub Profile README como um produto versionado. Conteúdo, apresentação, dados e automação permanecem separados para permitir evolução incremental, revisão simples e atualização segura.

## Estrutura

```text
README.md
assets/
├── brand/
├── svg/
├── images/
└── animations/
data/
docs/
scripts/
templates/
└──
.github/
└── workflows/
```

Arquivos `.gitkeep` mantêm no Git as pastas ainda vazias e serão removidos quando conteúdo real for adicionado.

## Responsabilidade das pastas

### `README.md`

Ponto de composição do perfil. Deve conter apenas a narrativa publicada, referências aos assets e marcadores controlados para conteúdo futuro. Não deve armazenar lógica de geração nem grandes blocos de dados.

### `assets/brand/`

Elementos canônicos da marca QA Orbit: logotipo, símbolos, arquivos-fonte da identidade e referências de paleta. O kit oficial fica em `assets/brand/qa-orbit/`, separado em `svg/`, `png/` e `source/`. Variações usam nomes explícitos por orientação, tratamento de cor e contexto. Os SVGs são a fonte oficial; PNGs são artefatos de exportação.

### `assets/svg/`

SVGs finais consumidos pelo README. A organização interna futura será feita por componente, com uma pasta compartilhada apenas quando um asset for realmente reutilizado.

Estrutura prevista:

```text
assets/svg/
├── shared/
├── hero/
├── system-status/
├── qa-orbit/
├── tech-stack/
├── projects/
├── statistics/
└── footer/
```

Convenções futuras:

- nomes em `kebab-case`;
- um asset deve ter uma responsabilidade visual clara;
- variantes recebem sufixos, como `-dark`, `-mobile` ou `-fallback`;
- IDs internos recebem o prefixo do componente;
- arquivos gerados devem ser identificáveis e reproduzíveis;
- código-fonte editável e artefatos finais não devem ser confundidos.

As subpastas previstas não são criadas nesta sprint porque ainda não existem assets; a convenção fica registrada antes da implementação.

### `assets/images/`

Imagens raster estáticas, capturas do produto, mockups e fallbacks de animações. Arquivos devem ser otimizados e nomeados por contexto, não por sequência genérica.

### `assets/animations/`

Arquivos animados publicados e, quando apropriado, seus arquivos-fonte. Animações compartilhadas serão tratadas como padrões reutilizáveis de movimento. Cada exportação deve registrar componente consumidor, fallback e finalidade.

Estrutura prevista:

```text
assets/animations/
├── shared/
├── hero/
└── qa-orbit/
```

Uma animação só será duplicada quando formatos ou dimensões diferentes forem necessários. Caso contrário, os componentes referenciarão o mesmo arquivo.

### `docs/`

Documentação de decisões, identidade, arquitetura e contratos de componentes. É a fonte de verdade para manutenção humana do perfil.

### `templates/`

Modelos reutilizáveis para assets ou fragmentos gerados. Templates não são publicados diretamente: scripts futuros os combinarão com dados validados.

### `scripts/`

Ferramentas determinísticas para validar dados, gerar assets e atualizar regiões controladas do README. Um script não deve editar conteúdo editorial fora de seus marcadores.

### `data/`

Dados estruturados que alimentam componentes dinâmicos, como status do QA Orbit, projetos selecionados e métricas. O conteúdo deve ser validável e independente da apresentação.

Estrutura futura possível:

```text
data/
├── profile.json
├── qa-orbit.json
├── projects.json
└── statistics.json
```

Esses arquivos serão criados somente quando seus contratos forem definidos.

### `.github/workflows/`

Automações futuras de atualização, validação e otimização. Workflows devem possuir permissões mínimas, comportamento previsível e nunca substituir todo o README desnecessariamente.

## Responsabilidade dos componentes

Cada componente corresponde a uma unidade narrativa do README. Seu contrato inclui:

- conteúdo editorial ou dados de entrada;
- apresentação estática ou asset associado;
- texto alternativo quando aplicável;
- limites claros de atualização automática;
- fallback para dependências visuais ou externas.

O inventário e as dependências específicas estão em `docs/components.md`.

## Fluxo futuro de dados

```text
Fontes confiáveis → coleta → validação → data/ → templates/ → assets ou região do README
```

Regras do fluxo:

1. Workflows coletam apenas dados necessários e autorizados.
2. Scripts normalizam e validam os dados antes de qualquer publicação.
3. Dados persistidos ficam separados do Markdown e da apresentação.
4. Templates transformam dados em uma saída determinística.
5. Apenas regiões explicitamente marcadas ou assets gerados são atualizados.
6. Uma falha preserva a última versão válida em vez de apagar conteúdo.
7. Mudanças automáticas devem produzir diffs pequenos e auditáveis.

## Evolução incremental

Cada sprint pode adicionar um componente sem exigir a implementação dos demais. Antes de integrar um componente ao README, devem existir:

- objetivo e conteúdo aprovados;
- regras visuais aplicáveis;
- asset otimizado, quando necessário;
- comportamento responsivo;
- fallback e texto alternativo;
- documentação atualizada.

## Escopo concluído na Sprint 1

A fundação inicial foi criada sem assets visuais, automações, dados dinâmicos, estatísticas, textos definitivos ou integrações externas. A partir da Sprint 2, componentes aprovados passam a ocupar as pastas previstas de forma incremental.
