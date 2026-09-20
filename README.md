# Diamond — Landing Page

Landing page de vitrine pra loja de camisas oversized **Diamond** (Vest Entregas), com pedidos feitos direto pelo WhatsApp.

## Estrutura

```
diamond-site/
├── index.html      → estrutura da página
├── style.css        → todo o estilo (cores, tipografia, responsivo)
├── script.js         → menu mobile (abre/fecha em telas pequenas)
├── README.md
└── img/
    ├── logo.png        → logotipo "Vest Entregas Diamond"
    ├── diamond.png      → ícone do diamante (usado no header/hero)
    ├── produto-1.png     → foto de produto (card 1 da coleção)
    ├── produto-2.png      → foto de produto (card 2 da coleção)
    └── produto-3.png       → foto de produto (card 3 da coleção)
```

## Como abrir

É só descompactar a pasta e abrir o `index.html` direto no navegador. Não precisa de servidor, build nem instalação — tudo é HTML/CSS/JS puro, sem framework.

## Seções da página

1. **Header** — logo + menu (Coleção, Sobre, Como comprar) + botão de WhatsApp
2. **Hero** — animação de entrada do diamante/logo, chamada principal e CTA
3. **Sobre** — versículo (Efésios 6:11) + texto da marca
4. **Coleção** — grade com as fotos dos produtos, cada uma com botão "Pedir no zap"
5. **Como comprar** — 3 passos (escolher → chamar no zap → receber em casa)
6. **Faixa de CTA** — chamada final antes do rodapé
7. **Footer** — logo, links de WhatsApp/Instagram

## O que já está configurado

- Número de WhatsApp: `5521965275735` (presente em todos os botões `wa.me`)
- Paleta de cores e fontes (Anton, Jost, Cormorant Garamond) seguindo a identidade da logo

## O que falta ajustar quando tiver a informação

- [ ] Trocar/adicionar mais fotos de produto em `img/` (os cards puxam de `produto-1.png`, `produto-2.png`, `produto-3.png` — pra adicionar um 4º card, duplica um bloco `.card` no `index.html` e ajusta o `grid-template-columns` no `style.css`)
- [ ] Confirmar o link do Instagram no rodapé (hoje está genérico: `instagram.com`)
- [ ] Preço e nome dos produtos, se quiser exibir (hoje os cards mostram só foto + botão)

## Deploy

Como é HTML/CSS/JS estático, sobe em qualquer hospedagem simples: Netlify, Vercel, GitHub Pages, ou até FTP num servidor comum. Basta subir a pasta inteira mantendo a estrutura de `img/` junto do `index.html`.