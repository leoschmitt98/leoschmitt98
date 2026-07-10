# QA Orbit brand source

Os SVGs em `../svg/` são os arquivos-fonte oficiais e autocontidos da marca v1.0 congelada. O desenho-base usa um `viewBox` de `0 0 256 256`; o favicon possui geometria simplificada própria.

## Arquivo canônico

`symbol-gradient.svg` é a implementação principal do símbolo. As versões monocromáticas e de lockup repetem a geometria deliberadamente para funcionar de modo isolado no GitHub, em navegadores e em produtos sem sprites ou referências externas.

## Exportação PNG recomendada

Os PNGs não foram gerados nesta sprint porque o ambiente não possui um rasterizador vetorial de produção instalado. Screenshots de navegador não oferecem garantia suficiente de transparência, escala e perfil de cor para serem tratados como exports oficiais.

Com Inkscape instalado, executar a partir da raiz do repositório:

```powershell
inkscape assets/brand/qa-orbit/svg/symbol-gradient.svg --export-filename=assets/brand/qa-orbit/png/symbol-512.png --export-width=512 --export-height=512
inkscape assets/brand/qa-orbit/svg/logo-horizontal-gradient.svg --export-filename=assets/brand/qa-orbit/png/logo-horizontal-1600.png --export-width=1600
inkscape assets/brand/qa-orbit/svg/logo-vertical-gradient.svg --export-filename=assets/brand/qa-orbit/png/logo-vertical-1200.png --export-width=1200
inkscape assets/brand/qa-orbit/svg/favicon.svg --export-filename=assets/brand/qa-orbit/png/app-icon-512.png --export-width=512 --export-height=512
```

O `social-preview.png` exigirá uma composição específica de 1200 × 630 px em uma sprint de aplicação da marca; ampliar o logo vertical não produziria um social card profissional.

## Controle de alterações

Mudanças na geometria-base devem ser replicadas em todas as variantes e acompanhadas por validação XML, renderização em fundos claro e escuro e testes em 16, 32, 64, 128 e 512 px.
