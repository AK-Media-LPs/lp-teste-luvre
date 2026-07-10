# 05-tracking — Códigos de rastreamento e destino do lead

## Arquivos
- **head.txt** — código pra inserir dentro do `<head>` da página final.
- **body.txt** — código pra inserir logo APÓS a abertura do `<body>`.

Os dois vieram do brief preenchido no TRACKR. Se estiverem com o comentário
de "nenhum código fornecido", peça os códigos ao responsável pelo tracking.

## Onde cada ferramenta entra (regra geral)
| Ferramenta | `<head>` | após `<body>` |
| --- | --- | --- |
| **Meta Pixel** | ✅ script completo (só no head) | ❌ nada |
| **GTM (Google Tag Manager)** | ✅ script (parte 1) | ✅ `<noscript>` (parte 2) |
| **GA4 (gtag.js direto)** | ✅ script completo | ❌ nada |
| **TikTok Pixel** | ✅ script completo | ❌ nada |

- Meta Pixel: **só no head**. Eventos de conversão (Lead/Purchase) disparam
  no clique do CTA ou na página de obrigado — combinar com o gestor.
- GTM: **pede head E body** — as duas partes vêm juntas no painel do GTM.
- GA4 via GTM: só o GTM na página; o GA4 configura-se dentro do painel.

## Destino do lead deste cliente
**Só checkout — a página NÃO captura lead; todo CTA aponta direto pro link de pagamento**

Detalhe/URL: https://pay.exemplo.com/dtg-97

O formulário/CTA da página final precisa apontar pra esse destino antes de
publicar — o Claude Design deixa o formulário pronto, mas a integração
(URL do webhook, link do checkout, embed do Kommo) é conferida pelo gestor.
