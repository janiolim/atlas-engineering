---
title: "Desenvolvimento de Fibras Compósitas MoS₂/CFO/PVP via SBS"
description: "Incorporação de dissulfeto de molibdênio e ferrita de cobalto em matriz polimérica para geração de materiais multifuncionais."
category: "research"
thumbnail: "./mos2-cfo-pvp.jpg"
tech:
  - SBS
  - Materiais Magnéticos
  - Compósitos
order: 8
publishDate: 2026-07-04
---

## Brief

A engenharia de materiais avançados busca a sinergia entre propriedades magnéticas (CFO) e características estruturais/eletrônicas bidimensionais (MoS₂) dispersas em uma matriz flexível (PVP).

## Approach

Preparação de uma suspensão homogênea contendo as nanopartículas e o polímero seguida do processamento por Solution Blow Spinning para a fiação de compósitos com alta dispersão de fases e forte acoplamento magnético.

```ts
export const checkCompositeDispersity = (loadingPercentage: number) => ({
  agglomerationRisk: loadingPercentage > 15,
  applicationScope: 'Flexible magnetic sensors or electromagnetic shielding coatings.'
});