# ImagineUP

Site público do ImagineUP, o app de fãs dos artistas da Imagine Music. O painel administrativo do app vai ser construído neste mesmo repositório.

## Site

HTML, CSS e JavaScript puros, sem etapa de build. Tudo fica na pasta `site/`:

| Endereço | Página |
| --- | --- |
| `/` | Página inicial |
| `/baixar/` | Download do app, com código QR |
| `/sobre/` | Sobre |
| `/novidades/` | Novidades |
| `/faq/` | Perguntas frequentes |
| `/contato/` | Fale conosco |
| `/privacidade/` | Política de Privacidade |
| `/termos/` | Termos de Uso |

Para abrir no computador, com o Node instalado:

```bash
npx serve site
```

Qualquer hospedagem de arquivos estáticos serve para publicar: basta apontar para a pasta `site/`. O código QR da página Baixar aponta para a própria página, então funciona em qualquer domínio.

Na Vercel, `site/vercel.json` faz cada página ter um endereço só (com barra no fim) e guarda em cache as fontes e as telas do app.

## Antes de publicar

- Os textos da Política de Privacidade e dos Termos de Uso passam pela revisão do jurídico da Imagine Music.
- Quando o app estiver nas lojas, preencher os links da App Store e do Google Play em `LOJAS`, no script de `site/baixar/index.html`, e nos links iOS e Android do rodapé de cada página. Com os links preenchidos, quem abre a página Baixar no celular vai direto para a loja certa.
