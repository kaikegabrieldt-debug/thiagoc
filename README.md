# Dr. Thiago Costa — Endocrinologia & Saúde Metabólica

Site institucional (landing page) do **Dr. Thiago Costa**, médico endocrinologista (CRM 27533-SC), com foco em
**Emagrecimento · Hormônios · Menopausa · Longevidade**. Atendimento em **Itapema/SC** e por **teleconsulta**.

Site **estático** (HTML + CSS + JavaScript puro, sem build e sem dependências) — rápido, acessível e fácil de manter.

## Estrutura

```
.
├── index.html          # Página única (todas as seções)
├── css/styles.css      # Design tokens + estilos
├── js/main.js          # Menu mobile, header sticky, scroll-reveal
├── assets/
│   ├── logo.svg        # Monograma TC (versão standalone)
│   ├── favicon.svg     # Ícone do navegador
│   └── img/            # Fotos (ver assets/img/README.md)
├── .nojekyll           # Publica os arquivos como estão no GitHub Pages
└── README.md
```

## Rodar localmente

Não precisa de build. Basta servir a pasta:

```bash
# Python 3
python -m http.server 8000
# depois abra http://localhost:8000
```

Ou simplesmente abra o `index.html` no navegador.

## Personalizar conteúdo

- **Fotos:** veja `assets/img/README.md`. Coloque os arquivos (`dr-hero.jpg`, `dr-sobre.jpg`, `og-image.jpg`) e
  troque os blocos marcados `<!-- FOTO: ... -->` no `index.html` pela tag `<img>` indicada.
- **Bio:** há um `<!-- TODO (Dr. Thiago) -->` na seção "Sobre" para personalizar formação e diferenciais.
- **Contato:** WhatsApp `+55 47 99167-2587` e Instagram `@dr.thiago.costa` já estão configurados nos links.
- **Cores/tipografia:** centralizadas nas CSS custom properties no topo de `css/styles.css`.

## Publicar no GitHub Pages

1. Suba o código para o repositório (ex.: `kaikegabrieldt-debug/thiagoc`), branch `main`.
2. No GitHub: **Settings → Pages → Build and deployment → Source: Deploy from a branch**.
3. Selecione branch **`main`** e pasta **`/ (root)`** e salve.
4. Em ~1 min o site fica disponível em `https://kaikegabrieldt-debug.github.io/thiagoc/`.

> Domínio próprio (ex.: `drthiagocosta.med.br`) pode ser adicionado depois em **Settings → Pages → Custom domain**.

## Conformidade

Conteúdo com caráter informativo e em linha com a publicidade médica do CFM: CRM visível, sem promessa de
resultados e sem imagens de antes/depois.
