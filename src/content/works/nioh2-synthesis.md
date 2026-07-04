---
title: "Síntese Hidrotermal de Ni(OH)₂ Nanoestruturado"
description: "Obtenção controlada de nanopartículas de hidróxido de níquel com foco na otimização de área superficial para eletrodos."
category: "research"
thumbnail: "./nioh2-synthesis.jpg"
tech:
  - Ni(OH)₂
  - Síntese Química
  - Eletroquímica
order: 7
publishDate: 2026-07-04
---

## Brief

Dispositivos de alto desempenho para armazenamento de energia eletroquímica dependem diretamente da redução de escala e do aumento da área superficial ativa dos nanomateriais constituintes.

## Approach

Utilização da rota sintética hidrotermal para forçar o crescimento nucleado de fases cristalinas puras de $\alpha$ ou $\beta$-Ni(OH)₂, controlando o pH do meio reacional e o tempo de residência no autoclave.

```ts
export const assessSynthesisPhase = (pH: number, temperatureC: number) => ({
  expectedPhase: pH > 11 && temperatureC >= 120 ? 'Beta-Ni(OH)2 plates' : 'Alpha-Ni(OH)2 turbostratic flakes',
  electrochemicalPotential: 'Alpha phase typically exhibits superior theoretical capacitance.'
});