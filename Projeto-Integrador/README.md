# Portfólio Pessoal — Pietro Correa

**Curso:** Desenvolvimento de Sistemas
**Unidade Curricular:** LIMA – Linguagem de Marcação
**Modalidade:** Projeto Integrador baseado em Competências (MSEP)

## Objetivo

Apresentar projetos, habilidades, interesses e formas de contato de forma clara e
atrativa, funcionando como vitrine profissional para recrutadores, colegas e
empresas. Público-alvo: recrutadores, professores e outros estudantes da área de tech.

## Tecnologias

- **HTML** — estrutura semântica (`header`, `nav`, `main`, `section`, `footer`)
- **CSS** — estilização, responsividade e recursos avançados
- **JavaScript (1 linha)** — so pro botão de impressão (`window.print()`)

## Estrutura do projeto

```
Projetin/
├── index.html          # estrutura do site
├── css/
│   └── style.css       # estilização 
├── images/
│   └── burguer.svg   # foto do site da Burguer Analytics
│   └── crm.svg       # foto do ProjetoCRM
│   └── logo.png      # logo da catina
│   └── perfil.jep    # minha foto de perfil
└── README.md           # este arquivo
```

## Recursos obrigatórios aplicados e onde foram usados

| Recurso | Onde foi utilizado |
|---|---|
| Gradientes (`linear-gradient`) | `#hero` (fundo), `.btn` (botões), `.social` (links de conexão), `footer` (rodapé) |
| Múltiplos backgrounds | `#hero`: 2 `radial-gradient` + 1 `linear-gradient` empilhados |
| CSS Columns (`column-count` / `column-gap`) | Seções "Sobre mim" e "Interesses pessoais" (`.colunas`) |
| Transformações 2D | `scale()` no `.btn` e `.card:hover`; `rotate()` no `.card:hover`; `translate()` no `.menu a:hover`, `.btn-print:hover` e `.social:hover` |
| Transition | `.menu a`, `.btn`, `.btn-print`, `.card`, `.social` |
| Animation (`@keyframes`) | `.avatar` — animação `flutuar` (foto de perfil sobe e desce) |
| Border image | `.btn-print` (botão "Imprimir / Salvar PDF") |
| Cores hex / RGB / RGBA / currentColor | hex: `#334589`, `#323A57`, `#BBC6F0`, `#D1DAFF`, `#9EB1FF`; rgb: `.card` e `.tags`; rgba: `header`, `.frase`, gradientes do hero; currentColor: borda dos `.badges li` |
| Seletores CSS | elemento: `body`, `h2`, `section`; classe: `.card`, `.btn`; id: `#hero`, `#contato`; agrupados: `h1, h2, h3`; avançados: `.menu a:hover`, `.badges li:hover`, `a::after` no print |
| Estilo para impressão | `@page` (A4, margem 2cm) + `@media print` no fim do CSS; botão "Imprimir / Salvar PDF" no hero |
| Fontes personalizadas | Ver seção "Fontes personalizadas" abaixo |

## Fontes personalizadas (@font-face)

A fonte personalizada já está configurada no CSS com `@font-face` (requisito do
professor), usando a origem `local()` — ou seja, o site usa a Poppins quando ela
está instalada no computador, sem precisar de pasta `fonts/`.

Para usar a Poppins em **qualquer** máquina, faça o seguinte:

1. Baixe a fonte **Poppins** (gratuita, Google Fonts): https://fonts.google.com/specimen/Poppins
2. Crie a pasta `fonts/` na raiz do projeto e coloque dentro `Poppins-Regular.ttf`
3. No `css/style.css`, troque a linha do `src` para:

```css
src: url("../fonts/Poppins-Regular.ttf") format("truetype");
```

Enquanto a Poppins não existir no computador, o site usa o Arial (fallback do `font-family`).

## Versão para impressão

O botão **"Imprimir / Salvar PDF"** no topo do site chama `window.print()`.
A versão impressa (`@media print` + `@page`) oculta menu, botões, foto e rodapé,
remove cores de fundo e animações, e mostra o endereço real dos links de conexão.

## Links apresentados no site

- GitHub: https://github.com/Pietro-Olimpio
- WhatsApp: https://wa.me/5519995752812
- LinkedIn: https://www.linkedin.com/in/pietro-correa

## Como visualizar

Basta abrir o `index.html` no navegador (duplo clique).

**Foto de perfil:** troque o arquivo `images/profile.svg` pela sua foto (ex.: `profile.jpg`)
e atualize o `src` da tag `<img class="avatar">` no `index.html`.

**Imagens dos projetos:** imagens tiradas de sites que eu ja fiz, somente uma (ProjetoCRM) foi criada com IA.
