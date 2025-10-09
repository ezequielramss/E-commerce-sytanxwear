# SyntaxWear — E-commerce (Frontend)

Projeto de front-end para uma loja online de tênis e sneakers, com layout responsivo, grid de produtos, seção hero e footer com newsletter.

Visão geral
-----------
- Stack: HTML5, CSS (arquivos organizados por componentes) — sem Javascript neste repositório.
- Estrutura pensada para ser estática e facilmente integrada a um backend ou gerador de sites.

Estrutura do projeto
--------------------
Raiz do projeto (principais arquivos/pastas):

- `index.html` — página principal do site.
- `css/`
	- `reset.css` — reset de estilos do navegador.
	- `base.css`, `layout.css` — estilos globais e layout.
	- `components/` — estilos componentizados:
		- `header.css` — estilos do cabeçalho e navegação responsiva.
		- `hero.css` — seção hero (banner).
		- `product-grid.css` — grid de produtos e variações.
		- `product-category.css` — cards de categoria.
		- `footer.css` — estilos do rodapé e newsletter.
		- `variables.css` — variáveis de cores/typography.
- `images/` — imagens usadas (logo, ícones, produtos, banners).

Como abrir localmente
---------------------
1. Clone o repositório ou baixe os arquivos.
2. Abra o `index.html` no navegador (duplo clique) ou sirva com um servidor local para evitar restrições de CORS com fontes/requests:

```pwsh
# Exemplo com Python 3
python -m http.server 3000
# então abra http://localhost:3000
```

Boas práticas e observações
--------------------------
- As dimensões no CSS usam `rem` para escalabilidade (assegure-se da `font-size` base no `html` se precisar de valores precisos).
- Componentes são isolados em `css/components/` para facilitar manutenção e reuso.
- O menu responsivo atual usa um checkbox (`.menu-toggle`) como controle off-canvas. Para melhorar acessibilidade, é recomendado trocá-lo por um botão com `aria-expanded` controlado via JS.

Checklist rápida para desenvolvimento
-----------------------------------
- [ ] Validar HTML com o W3C Validator
- [ ] Otimizar imagens (WebP e compressão) em `images/products/`
- [ ] Adicionar SVGs inline para ícones (melhora performance e styling)
- [ ] Implementar pequenas interações com JS (menu acessível, filtro de produtos)

Sugestões de próximos passos
----------------------------
- Transformar os componentes em includes (templates) caso vá usar um backend (e.g., Express, Jekyll, etc.).
- Adicionar testes visuais (Percy, Chromatic) e lint de CSS/HTML.
- Preparar rotas e endpoints para integração com API de produtos.

Contatos
--------
Se quiser, posso:

- ajustar o menu para ser totalmente acessível com um botão + JS;
- otimizar o CSS e transformar em Sass/SCSS;
- gerar um arquivo de deploy (Netlify/Vercel) com instruções.

---
Arquivo gerado automaticamente pelo assistente — revise e ajuste os caminhos/imagens conforme necessário.
