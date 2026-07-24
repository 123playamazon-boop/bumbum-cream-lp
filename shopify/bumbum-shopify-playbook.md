# BUMBUM — Shopify Scaling Playbook
### LTV (assinatura) · AOV (bundles/upsell) · Recuperação de carrinho · Prova social
*Pesquisa jul/2026 — aplicada à nossa página DR (advertorial + DTC, oferta 1/2/3 potes $59/$79/$89).*

---

## TL;DR — o stack que eu recomendo pra começar (barato, escala depois)

| Função | App recomendado (começo) | Escala | Por quê |
|---|---|---|---|
| **Assinatura (LTV)** | **Appstle** (grátis→baixo) ou Seal (grátis) | Loop / Recharge | Full-featured, barato pra loja nova. Recharge comprou a Skio (abr/26) → mercado é Recharge vs Loop no topo |
| **Upsell pós-compra (AOV)** | **AfterSell** | Zipify OCU (funis multi-step) | Melhor cobertura + A/B nativo. **Evitar ReConvert** (em 2026 exibiu anúncios de terceiros no thank-you sem consentimento) |
| **Recuperação carrinho** | **Klaviyo** (email+SMS) + PushOwl (push grátis) | + Recart (SMS gerenciado) | Padrão da indústria, melhor segmentação. Receita recuperada costuma ser 15–30× o custo do app |
| **Reviews com foto (UGC)** | **Loox** | Okendo (premium) | +8–12% de conversão na página; foto/vídeo vale 5–8× texto e **vira criativo de Meta** |
| **Cart / "frequently bought"** | AfterSell cart | Rebuy (IA, $1M+/mês) | Aumenta AOV no carrinho |

Em volume baixo dá pra rodar quase tudo em plano grátis/baixo; Klaviyo e Loox escalam com contatos/pedidos.

---

## 1) Assinatura = a maior alavanca de LTV

Assinatura ("Subscribe & Save") transforma 1 compra em receita recorrente. Em beleza, assinatura chega a **25–40% do faturamento**.

**Como fazer certo (dados de churn):**
- **Desconto 15% recorrente** — o ideal é 10–15%. Fundo demais (30–40% na 1ª) atrai caçador de promoção que cancela rápido.
- **Dual-pricing**: 20% na 1ª entrega + 15% nas seguintes = incentivo de aquisição sem viciar em desconto.
- **3–4 opções de frequência** (30/45/60/90 dias) → **23% menos churn** que só "mensal".
- **Pausar/pular/trocar fácil** = a maior alavanca de retenção. "Quem consegue pausar, não cancela."
- SMS/email **"acabando seu potinho?"** antes do próximo envio → -15–18% de skip.
- Migrar de desconto pra **valor** (brinde na 1ª, acesso antecipado) retém melhor.

**Na nossa página:** adicionar um toggle **"Comprar uma vez / Assinar e economizar 15%"** em cada card da oferta 1/2/3 potes. O 2 potes (most popular) vira a âncora da assinatura ("seu ciclo de 60 dias, sempre 15% off, cancele quando quiser").

---

## 2) AOV — bundle, quantity breaks e upsell

- **Bundle = a maior alavanca de AOV em beleza.** Bundles de "rotina/resultado" convertem **2–3×** e sobem AOV **+30–45%** vs produto único. Nossa oferta 1/2/3 já é quantity-break — falta **enquadrar como "kit de resultado de 60/90 dias"**, não "compre 3 e economize".
- **Upsell pós-compra 1-clique** (adiciona ao pedido depois do pagamento, sem redigitar cartão): **AfterSell** ou **Zipify OCU**. Ex.: após comprar, ofertar **+1 potinho com desconto** ou um **applicator/escova de massagem**.
- **Free-shipping bar / brinde por valor (GWP):** 83% dos compradores de beleza são movidos por frete grátis (+15–28% AOV). Já temos frete grátis — dá pra somar um **"brinde grátis acima de $X"** pra empurrar do 2 pro 3 potes.
- **"Frequently bought together" / cart upsell:** Rebuy (IA) quando escalar; AfterSell no carrinho pra começar.

---

## 3) Recuperação de carrinho (o motivo principal de ir pro Shopify)

O Stripe Payment Link não recupera nada. No Shopify:
- **Abandoned checkout nativo** (grátis, baseline) — liga já.
- **Klaviyo** (email+SMS num lugar só, melhor segmentação, ~$20/mês inicial). Fluxos essenciais: **checkout abandonado, browse abandon, pós-compra, winback**.
- **PushOwl** (push no navegador) — alcança quem **nunca deu e-mail nem telefone**, só aceitou o push.
- Escala de SMS: **Recart** (gerenciado, ~$299/mês, pra $100k+/mês).

Regra prática: em qualquer faixa, a **receita recuperada supera o custo do app em 15–30×**.

---

## 4) Prova social / reviews (converte E alimenta anúncio)

- Produto com **10+ reviews converte 52% mais**; review com **foto/vídeo vale 5–8×** texto.
- **Loox** — melhor captura de foto/vídeo, +8–12% de conversão na página, e as fotos **viram criativo de Meta** (perfeito pro nosso ângulo antes/depois). Alternativa grátis: **Judge.me**. Premium/segmentação: **Okendo**.
- **Na nossa página:** trocar os depoimentos estáticos por widget do **Loox** (reviews reais com foto) + estrela agregada perto do título.

---

## 5) O que as lojas escaladas fazem (e a gente já tem / vai ter)

Marcas de corpo/beleza escaladas no Shopify (ex.: Bushbalm — skincare de bumbum/corpo, Sol de Janeiro, Truly) rodam basicamente: **quiz → PDP com UGC pesado → quantity-break/bundle → subscribe & save → upsell pós-compra → fluxos Klaviyo**.

Checklist de página (✓ = já temos):
- ✓ Sticky "Add to Cart" no mobile
- ✓ Quantity breaks com total + por-potinho + riscado
- ✓ Urgência/escassez (contador + barra de estoque)
- ✓ Carrossel 7+ imagens, antes/depois, garantia, selos
- ➕ Estrela agregada perto do título + 3–5 reviews acima da dobra (Loox)
- ➕ Toggle assinatura 15% em cada tier
- ➕ Barra de progresso "brinde grátis acima de $X"
- ➕ Upsell 1-clique pós-compra
- ➕ Fluxos de recuperação (Klaviyo + PushOwl)

---

## Ordem de implementação sugerida

1. **Você:** instalar os apps que topar (começo enxuto: **Appstle + AfterSell + Loox + Klaviyo**; PushOwl grátis).
2. **Eu:** criar o produto **Bumbum** com variantes 1/2/3 potes ($59/$79/$89) + **selling plan de assinatura** (15% recorrente / 20% na 1ª).
3. **Eu:** publicar nossa página como landing (template Liquid) com botões no carrinho + toggle de assinatura.
4. **Eu:** ligar upsell pós-compra (AfterSell), Loox na página, e desenhar os fluxos do Klaviyo.
5. **Eu:** Meta Pixel (canal Facebook) + Clarity + rechecar RedTrack no Shopify.

---

### Fontes
- Subscription apps / churn: recurpay.com, loopwork.co, easysubscription.io, appstoreresearch.com
- Upsell pós-compra: zipify.com, aftersell.com, skailama.com
- Recuperação de carrinho: libautech.com, recapture.io, getkanal.com
- Reviews: siteoptimizr.com, wiserreview.com, coreppc.com
- CRO beleza / AOV / PDP: easyappsecom.com, shopify.com, adsgun.com, ecorn.agency

---
---

# PARTE 2 — O que as lojas ESCALADAS fazem (jul/2026) → aplicar no Bumbum
*Estudei: Bushbalm (skincare de corpo/bumbum, bootstrap $900 → 8 dígitos) + padrões de DTC de beleza escalados.*

## As alavancas que as escaladas usam
1. **Quiz de diagnóstico** — captura **~40%** dos visitantes (vs 2–3% de formulário), 3–5 perguntas, recomenda o bundle e **personaliza e-mail/SMS** depois. Constrói **dado 1st-party** (vantagem enorme pós-iOS). → *maior alavanca NOVA pra nós.*
2. **SMS + e-mail = motor de retenção** — Bushbalm tira **$1.30 por SMS enviado**; captura telefone no checkout. Em marcas $5M+, **retenção = 50%+ do faturamento**.
3. **UGC/conteúdo + TikTok** — Bushbalm: **+600% de receita** via social; TikTok = 28% do spend. Foto/vídeo de cliente vira criativo de anúncio.
4. **Arquitetura de oferta** — bundle com economia clara; **frete grátis / brinde com gatilho 15–20% ACIMA do AOV** (empurra o ticket pra cima); upsell no PDP tipo "add X por +$Y, economize 15%"; assinatura.
5. **GWP (brinde) > desconto fundo** — brinde na 1ª compra retém melhor que "50% off", que atrai caçador de promoção que cancela.
6. **Cuidado com upsell pós-compra** — ajuda o AOV no painel, mas pode **canibalizar o LTV**; bundle + assinatura são mais duráveis. Usar com teto.
7. **Marca/missão forte** — Bushbalm quebrou o tabu de "corpo"; nós temos a história **It's Brazilian / Amazônia** — usar como diferencial, não rodapé.

## Aplicar no Bumbum (priorizado)
1. **[GRANDE] Quiz "Descubra seu plano de firmeza em 20s"** — 3–4 perguntas (idade · queixa: celulite/flacidez/estrias · há quanto tempo · meta de prazo) → recomenda **2 ou 3 potes** + **captura e-mail/telefone** → joga na oferta. Precisa de endpoint de captura (Klaviyo/Formspree).
2. **[GRANDE] Subscribe & Save 15%** (app Appstle) — receita recorrente / LTV.
3. **[MÉDIO] Brinde digital REAL (GWP)** — eu crio um **"Guia do Ritual Brazilian Lift" (PDF)** grátis com 2+ potes, entregue por e-mail. Honesto (a gente entrega) e empurra pro 2/3 potes.
4. **[RÁPIDO] Reframe de bundle + value-stack** — 1 pote = "Starter", 2 = "Kit Resultado 60 dias" (most popular), 3 = "Kit Ciclo Completo 90 dias"; bloco "o que vem no seu kit: creme + guia + garantia 60d + frete grátis".
5. **[APP] UGC reviews (Loox)** — foto real que sobe conversão e vira criativo de Meta.
6. **SMS/e-mail** — captura no quiz + checkout → fluxos Klaviyo (abandonado, "acabando o potinho", winback).

### Fontes (Parte 2)
- Bushbalm: shopify.com/case-studies/bushbalm, shopify.com/blog/bushbalm-marketing, adexchanger.com
- Oferta/AOV/retenção: peelinsights.com, elevate-digital-solutions.com, askneedle.com
- Quiz funnel: convertflow.com, heyflow.com, pennock.co
