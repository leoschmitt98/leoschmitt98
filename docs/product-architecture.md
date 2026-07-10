# Product Architecture

## Objetivo

Explicar como uma pessoa de QA percorre o QA Orbit no trabalho diário. A seção representa a experiência e a visão do produto, não a arquitetura técnica ou o estado exato de implementação de cada módulo.

## Modelo da experiência

O fluxo foi organizado em quatro fases cognitivas:

```text
Discover → Build → Validate → Learn ↺
```

As fases reduzem nove etapas a um modelo que pode ser compreendido rapidamente:

1. **Discover:** transformar intenção de produto em contexto e plano.
2. **Build:** capturar fluxos, construir automação e ampliar decisões com IA.
3. **Validate:** executar e preservar evidências.
4. **Learn:** reter conhecimento e alimentar o próximo ciclo.

## Ordem das etapas

### Discover

1. **Requirements:** estabelece o contexto que será validado.
2. **Test Planning:** converte esse contexto em risco, prioridade e cobertura.

### Build

3. **Smart Recorder:** captura a experiência real como entrada estruturada.
4. **Automation Builder:** transforma entradas em cenários reutilizáveis.
5. **QA Agent:** analisa o contexto reunido e apoia decisões.

### Validate

6. **Execution:** coloca o plano e a automação em contato com o produto.
7. **Evidence:** preserva os sinais necessários para compreender o resultado.

### Learn

8. **History:** mantém decisões, execuções e evidências acessíveis.
9. **Continuous Improvement:** devolve o aprendizado ao início do fluxo.

Essa ordem demonstra que o QA Orbit não termina na execução. O resultado de um ciclo torna-se contexto para o próximo.

## Estrutura de cada etapa

Cada bloco possui apenas três elementos:

- **Nome:** identifica a etapa ou módulo.
- **Objective:** descreve a intenção da ação.
- **Result:** mostra o valor produzido para a etapa seguinte.

Os textos não descrevem telas, integrações ou funcionalidades ainda não confirmadas. Eles registram a visão conceitual do produto.

## Decisões de UX

- A frase inicial explica o ciclo antes dos detalhes.
- Quatro fases funcionam como landmarks visuais e reduzem carga cognitiva.
- A numeração de `01` a `09` elimina a necessidade de setas ou diagrama.
- Objective e Result estabelecem causa e consequência em todas as etapas.
- Os blocos usam Markdown nativo para manter leitura linear e acessível.
- O fechamento retoma a ideia de ciclo sem repetir o manifesto da seção anterior.
- Nenhum SVG foi criado porque não adicionaria informação ao modelo numerado.

## Responsividade

### Desktop

As fases criam pausas visuais e os blocos formam uma sequência vertical fácil de escanear. Não há diagrama largo nem texto em colunas.

### Tablet

A ordem e a hierarquia permanecem idênticas. O layout depende apenas do container responsivo do GitHub.

### Mobile

Cada etapa ocupa uma coluna e mantém nome, objetivo e resultado juntos. Não existem medidas fixas, tabelas, imagens ou conteúdo que exija rolagem horizontal.

## Acessibilidade

- Toda informação importante está em Markdown.
- A hierarquia de headings acompanha a estrutura do README.
- A ordem visual é a mesma ordem de leitura.
- Fases e etapas não dependem de cor ou ícones.
- Objective e Result possuem labels textuais explícitas.

## Assinatura

> Every signal strengthens the next cycle. Quality keeps moving with the product.

A assinatura comunica aprendizado contínuo e proximidade com a evolução do produto sem tratar qualidade como uma etapa final.

## Escopo

Esta sprint adiciona somente a seção Product Architecture e sua documentação. Não altera Hero, Brand Kit, seção de produto existente ou placeholders das próximas sprints.
