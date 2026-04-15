# CLAUDE.md — OCTOOC

Site gerado pelo **SF (Site Factory)** em 15/04/2026.

## Contexto do Site

**Nome:** OCTOOC
**Nicho:** Tecnologia
**Keywords:** Somos uma empresa de prestacao de servicos no ramo tecnologico voltada para
**Paleta de cores:** forest | **Fonte:** lora

Somos uma empresa de prestação de serviços no ramo tecnológico voltada para o cliente final. Percebemos a necessidade das pessoas em ter a melhor tecnologia disponível no mercado e estamos aqui para fazer esta curadoria por você. Hoje em dia a tecnologia está em vários momentos do seu dia a dia, portanto, saber qual você vai usar pode significar ganho de produtividade, ganho financeiro e destaque profissional. É praticamente impossível você sozinho acompanhar todas as atualizações de mercado, aprender todas as novas funcionalidades de um novo aplicativo ou até mesmo entender qual é o melhor curso de capacitação para você, por isso estamos aqui para te ajudar e facilitar a sua vida com: Tutoriais exclusivos Indicações de novas tecnologias Tudo sobre Criptomoedas Indicações de cursos de Capacitações Consultorias com profissionais capacitados. A OcTooC é uma empresa voltada para te guiar quando o assunto é tecnologia. Mais do que um site de consultas, nós somos o caminho mais curto para você encontrar o que há de melhor no mercado tecnológico e facilitar o seu dia a dia.



## Componentes visuais usados

| Seção | Variante |
|-------|----------|
| Header | Header-D |
| Hero | Hero-C |
| Features | Features-D |
| About Section | About-E |
| Posts | Posts-C |
| Footer | Footer-D |
| Página Sobre | Sobre-B |
| Página Contato | Contato-I |

## Estrutura do projeto

```
src/
  sections/        # Layout escolhido pelo SF — Header, Hero, Features, About, Posts, Footer, Sobre, Contato
  data/            # JSONs com todo o conteúdo editável
  content/blog/    # Posts em Markdown
  pages/           # Rotas Astro (index, sobre, contato, blog, privacidade, termos)
  layouts/         # BaseLayout com fonte e cores dinâmicas
  styles/          # global.css com variáveis CSS de cor
public/
  images/          # hero.jpg, about.jpg, blog/*.jpg — inseridos automaticamente via Pexels
```

## O que editar

### Textos e conteúdo
- **`src/data/home.json`** — hero (título, subtítulo, botão), features (título, items), about section (título, desc, stats), posts
- **`src/data/sobre.json`** — conteúdo completo da página Sobre (hero, texto, missão)
- **`src/data/contato.json`** — título, subtítulo, email, tempo de resposta
- **`src/data/siteConfig.json`** — nome, slug, email, redes sociais, menu

### Imagens
Imagens já estão em `public/images/` (via Pexels). Para substituir, mantenha os mesmos nomes de arquivo:
- `hero.jpg` — imagem de fundo do Hero
- `about.jpg` — imagem da seção About (home)
- `sobre.jpg` — imagem de fundo da página Sobre
- `blog/{slug}.jpg` — imagens dos posts

### Posts do blog
Arquivos em `src/content/blog/`. Ajuste o tom de voz, adicione dados específicos do nicho e personalize conforme a identidade do site.

### Cores
Variáveis em `src/styles/global.css`: `--color-primary`, `--color-accent`, `--color-dark`.

## Deploy

```bash
bun install
bun run build
# Faça upload da pasta dist/ para Netlify, Vercel ou hosting estático
```
