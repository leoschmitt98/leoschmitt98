# Catálogo de componentes

Este documento define o mapa inicial de componentes. Os nomes representam responsabilidades de produto, não uma obrigação de usar um framework ou gerar HTML.

## Hero

**Objetivo:** criar a primeira impressão e estabelecer Leonardo Schmitt como o engenheiro por trás do QA Orbit.

**Responsabilidade:** apresentar identidade, posicionamento e chamada principal sem detalhar todo o perfil.

**Arquivos envolvidos:** `assets/svg/hero/hero-static.svg`, `assets/svg/hero/hero-animated.svg`, `docs/hero.md` e `README.md`.

**Dependências:** identidade visual, especificação registrada em `docs/hero.md`, marca oficial definida em `docs/qa-orbit-brand-guide.md` e regras de acessibilidade. A primeira versão estática foi criada na Sprint 2 e ainda não foi integrada ao README; sua atualização com o símbolo oficial será uma sprint posterior.

## SystemStatus

**Objetivo:** comunicar que o ecossistema e o projeto principal estão ativos.

**Responsabilidade:** exibir poucos sinais de contexto, como função, foco, projeto principal e estado atual.

**Arquivos envolvidos:** futuro `assets/svg/system-status/`, `data/qa-orbit.json`, templates e scripts de geração.

**Dependências:** QAOrbit, contrato de dados, fontes confiáveis e automação futura. Não está presente no README inicial.

## Mission

**Objetivo:** explicar a visão de Leonardo sobre qualidade de software.

**Responsabilidade:** conectar QA, automação, desenvolvimento e IA em uma narrativa curta, sem formato de currículo.

**Arquivos envolvidos:** `README.md` e, apenas se aprovado futuramente, assets de apoio.

**Dependências:** posicionamento editorial e proposta de valor do QA Orbit. Na estrutura inicial, é representado pela pequena apresentação.

## QAOrbit

**Objetivo:** posicionar o QA Orbit como o núcleo do perfil e principal produto em construção.

**Responsabilidade:** apresentar proposta de valor, capacidades, evolução e acesso ao projeto.

**Arquivos envolvidos:** `README.md` e `docs/product-section.md`. Assets, dados ou templates poderão ser adicionados somente quando houver uma necessidade funcional aprovada.

**Dependências:** Brand Kit oficial em `assets/brand/qa-orbit/` e narrativa documentada em `docs/product-section.md`. A primeira versão foi implementada em Markdown na Sprint 3; não depende de imagens, métricas ou automação.

## TechStack

**Objetivo:** demonstrar capacidade técnica como arquitetura integrada, não como coleção de logos.

**Responsabilidade:** organizar frontend, backend, automação e infraestrutura em camadas compreensíveis.

**Arquivos envolvidos:** `README.md`, futuro `assets/svg/tech-stack/` e possível arquivo de dados editorial.

**Dependências:** inventário tecnológico aprovado, linguagem visual e relação de cada tecnologia com a narrativa.

## ProductArchitecture

**Objetivo:** explicar como uma pessoa de QA percorre o fluxo conceitual do QA Orbit.

**Responsabilidade:** conectar requirements, planejamento, criação, assistência, execução, evidência, história e melhoria contínua em uma experiência única.

**Arquivos envolvidos:** `README.md` e `docs/product-architecture.md`.

**Dependências:** narrativa do produto em `docs/product-section.md`. A primeira versão foi implementada em Markdown na Sprint 4 e não depende de SVG, dados ou automação.

## Projects

**Objetivo:** apresentar evidências de execução por meio de projetos selecionados.

**Responsabilidade:** organizar projetos como missões, mantendo o QA Orbit em destaque e evitando listagem automática indiscriminada.

**Arquivos envolvidos:** `README.md`, futuro `assets/svg/projects/`, `data/projects.json` e templates de cards.

**Dependências:** curadoria de projetos, metadados consistentes, links públicos e template aprovado.

## Statistics

**Objetivo:** fornecer sinais relevantes de atividade e evolução.

**Responsabilidade:** exibir somente métricas com contexto, procedência e valor narrativo.

**Arquivos envolvidos:** `README.md`, futuro `assets/svg/statistics/`, `data/statistics.json`, scripts e workflows.

**Dependências:** fontes de dados confiáveis, regras de atualização, tratamento de falhas e design aprovado. Nenhuma estatística é implementada nesta sprint.

## CurrentTransmission

**Objetivo:** mostrar o foco atual de construção ou pesquisa.

**Responsabilidade:** publicar uma atualização curta e controlada sem transformar o perfil em um feed.

**Arquivos envolvidos:** futuro arquivo em `data/`, template, script e região delimitada no README.

**Dependências:** processo editorial ou fonte automatizada, contrato de dados e frequência de atualização. Não está presente no README inicial.

## Contact

**Objetivo:** converter interesse em uma ação clara.

**Responsabilidade:** oferecer canais de contato e colaboração com linguagem coerente com o QA Orbit.

**Arquivos envolvidos:** `README.md` e, futuramente, possível asset estático de apoio.

**Dependências:** canais aprovados, URLs definitivas e texto da chamada para ação.

## Footer

**Objetivo:** encerrar a experiência com uma assinatura visual consistente.

**Responsabilidade:** reforçar a marca sem repetir informações ou competir com o contato.

**Arquivos envolvidos:** futuro `assets/svg/footer/` e `README.md`.

**Dependências:** marca QA Orbit e composição final do Contact. Ainda não está presente no README inicial.

## Ordem sugerida de implementação

1. Hero e Mission.
2. QAOrbit.
3. SystemStatus.
4. TechStack e ProductArchitecture.
5. Projects.
6. Statistics e CurrentTransmission.
7. Contact e Footer.

Cada componente deve ser aprovado isoladamente antes de iniciar o próximo.
