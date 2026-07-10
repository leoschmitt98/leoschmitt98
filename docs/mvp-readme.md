# GitHub Profile — MVP

## Objetivo

Esta versão consolida o perfil em uma landing page curta e modular. Ela prioriza impacto visual, personalidade e leitura rápida, sem transformar o README em currículo ou documentação extensa do QA Orbit.

## Módulos publicados

1. Hero pessoal.
2. QA Orbit como projeto principal.
3. Beyond the role.
4. Quality engineering mindset.
5. Selected builds.
6. Engineering stack.
7. Public GitHub activity.
8. Contact.

## Estratégia de conteúdo

- Leonardo permanece como protagonista; o QA Orbit aparece como flagship.
- A seção de produto foi condensada em proposta, filosofia e fluxo conceitual.
- Informações profissionais usam somente dados fornecidos pelo proprietário do perfil.
- Sheila System usa dados confirmados no repositório público.
- QA Orbit e EJL System não recebem links ou métricas não verificadas.
- Cards do GitHub consultam dados públicos dinamicamente e não fixam números no README.
- LinkedIn e e-mail permanecem explicitamente pendentes até existirem URLs públicas aprovadas.

## Assets

Os banners em `assets/svg/sections/` compartilham:

- canvas de 1200 × 150;
- fundo Orbit Night;
- borda Orbit Border;
- tipografia segura;
- título, descriptor e motivo visual próprio;
- `<title>` e `<desc>` acessíveis;
- ausência de JavaScript e animações.

## Dependências externas

- `skillicons.dev`: faixa visual de tecnologias.
- `github-profile-summary-cards.vercel.app`: dados públicos de atividade, linguagens e estatísticas.

Esses componentes possuem texto alternativo. A indisponibilidade externa não remove o conteúdo editorial principal, mas pode ocultar temporariamente os cards dinâmicos.

## Responsividade

- Banners usam largura relativa e `viewBox` responsivo.
- Conteúdo editorial permanece em uma coluna.
- Cards de projetos usam blockquotes empilháveis.
- Tecnologias permanecem disponíveis em texto mesmo se os ícones não carregarem.
- Cards de estatísticas usam larguras relativas e podem empilhar conforme o renderer.

## Evoluções recomendadas

1. Integrar a marca v1.0 ao núcleo do Hero.
2. Criar variante mobile do Hero principal.
3. Adicionar URLs públicas de LinkedIn e e-mail.
4. Substituir cards externos por assets próprios gerados quando houver automação aprovada.
5. Publicar link ou demonstração do QA Orbit quando disponível.
6. Validar a identidade e a descrição pública do EJL System.
7. Refinar individualmente cada módulo após observar o README completo no GitHub.
