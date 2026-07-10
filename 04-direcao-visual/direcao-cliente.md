# Direção de design system — Teste LUVRE

> Escrita pelo Diretor de Arte do LUVRE em 09/07/2026. Isto é uma DIREÇÃO pro
> Claude Design **construir** o design system — não é CSS pronto nem paleta
> fechada em código. O Claude Design tem liberdade de execução dentro desta
> direção.

## Personalidade visual
Médico-editorial sofisticado: base off-white clínica, azuis do claro ao petróleo dando profundidade, tipografia display de peso. Confronta sem gritar — autoridade de quem executa.

## Sistema de cor
Cores da marca no brief: primária `#1476B0`, secundária `#0B3A5C`.

- `#F7FAFC` fundo off-white (base)
- `#FFFFFF` superfície de card
- `#1476B0` azul principal (ação/destaque)
- `#0B3A5C` azul petróleo (títulos e fundo de seção de contraste)
- `#5FA8D3` azul claro (camadas e gráficos)
- `#0F2438` tinta de texto
Proibido: preto+dourado, gradiente roxo, azul pastel chapado.

## Tipografia
**Par escolhido: Nohemi + Geist** (`nohemi-geist`)

| Papel | Fonte | Download | Licença |
| --- | --- | --- | --- |
| Display (headlines) | Nohemi | https://rajputrajesh-448.gumroad.com/l/NOHEMI9 | Grátis pra uso pessoal e comercial (pay-what-you-want, Rajesh Rajput). Espelho: https://fontesk.com/nohemi-typeface/ |
| Texto (corpo) | Geist | https://vercel.com/font | SIL Open Font License 1.1 (Vercel) — https://github.com/vercel/geist-font |

Nohemi pra headlines (peso 700-800 na linha 2 do hero, 500 na linha 1 — contraste real), Geist pro corpo (400/500) e números tabulares nas stats. Escala fluida com clamp: hero ~clamp(2.2rem, 6vw, 4.5rem).

## Componentes
CTA sólido azul principal com sombra em camadas; cards de dor com borda 1px e barra de status; selos em fileira horizontal com ícone linear; stat de destaque com zero à esquerda (ex.: "07 dias") em Nohemi 800.

## Elemento-assinatura
Peça de SERP (resultado de busca Google) estilizada: no hero, o concorrente aparece no topo e a clínica do leitor apagada abaixo; ao longo do scroll as posições se aproximam; perto do CTA final a clínica assume o topo. É o arco visual da promessa.

## Motion
Scroll-driven como espinha: a SERP evolui amarrada ao scroll (scrub), parallax multicamada na seção de problema, mask reveal linha a linha nas headlines, e o momento pinado na inversão da SERP (única seção de ousadia). Cards com reveal escalado alternado.

## Logo
Sem logo fornecido — usar marca tipográfica com a fonte display.
