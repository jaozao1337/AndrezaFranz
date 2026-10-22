# Site · Andreza Franz Estética

Site de cursos da Andreza Franz Estética (Caçador – SC): página inicial com o catálogo e uma página para cada curso.

## Arquivos

- `index.html`: página inicial (catálogo, sobre, dúvidas e contato)
- `limpeza-de-pele.html`: Curso de Limpeza de Pele
- `extensao-de-cilios.html`: Curso de Extensão de Cílios
- `design-de-sobrancelhas.html`: Curso de Design de Sobrancelhas
- `css/site.css`: cores, fontes e layout de todas as páginas
- `favicon.ico`: ícone da aba do navegador (deixe na raiz, ao lado dos `.html`)
- `img/`: fotos, logo, ícones do site em tamanhos maiores (`favicon-32.png`, `favicon-192.png`, `apple-touch-icon.png`) e imagens de prévia de link (`og-*.jpg`)

Mantenha as pastas `css` e `img` ao lado dos arquivos `.html`, com esses mesmos nomes.

## Publicar no GitHub Pages

1. Crie um repositório **público** no GitHub (ex.: `andreza-franz-site`).
2. Na página do repositório, clique em **Add file → Upload files** e arraste todos os arquivos `.html`, o `favicon.ico`, o `README.md` e as pastas `css` e `img` inteiras. Clique em **Commit changes**.
3. Vá em **Settings → Pages**. Em **Build and deployment**, escolha **Deploy from a branch**, branch `main`, pasta `/ (root)`, e clique em **Save**.
4. Em alguns minutos o site fica no ar em `https://SEU-USUARIO.github.io/andreza-franz-site/`.

Cada curso tem seu próprio link para mandar no WhatsApp, por exemplo `.../extensao-de-cilios.html`.

## Domínio próprio

1. Em **Settings → Pages → Custom domain**, digite o domínio (ex.: `andrezafranz.com.br`) e clique em **Save**. Faça isso antes de mexer no DNS.
2. No painel onde o domínio foi registrado (Registro.br, Hostinger etc.), crie os registros de DNS:
   - Domínio principal: quatro registros **A** apontando para `185.199.108.153`, `185.199.109.153`, `185.199.110.153` e `185.199.111.153`
   - `www`: um registro **CNAME** apontando para `SEU-USUARIO.github.io` (sem o nome do repositório)
3. Quando aparecer a opção (pode levar até 24 horas), marque **Enforce HTTPS**.

## Prévia de link no WhatsApp

Para a foto aparecer quando o link for compartilhado, troque em cada arquivo `.html` a linha:

```html
<meta property="og:image" content="img/og-image.jpg">
```

pelo endereço completo, por exemplo:

```html
<meta property="og:image" content="https://andrezafranz.com.br/img/og-image.jpg">
```

## Onde mudar as informações mais comuns

Use a busca do editor (Ctrl+F) nos arquivos `.html`:

- **Preços**: procure `1.500`, `1.200` ou `900` (aparecem no catálogo da página inicial e na página do curso)
- **WhatsApp**: procure `5549999190011` (links) e `99919-0011` (número exibido)
- **Endereço**: procure `Manoel Frâncio`
- **Avaliações do Google**: procure `10 avaliações` e atualize o número quando chegarem novas
- **Mensagens automáticas do WhatsApp**: ficam no fim dos links `wa.me/...?text=`
