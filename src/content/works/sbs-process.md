---
title: "Otimização de Parâmetros na Síntese de Nanofibras via SBS"
description: "Estudo experimental focado no controle de diâmetro e homogeneidade de mantas poliméricas geradas por sopro em solução."
category: "research"
thumbnail: "./sbs-process.jpg"
tech:
  - SBS
  - Nanofibras
  - Reologia de Polímeros
order: 6
publishDate: 2026-07-04
---

## Brief

A produção de membranas nanoestruturadas exige um rígido controle morfológico das fibras para garantir reprodutibilidade em aplicações tecnológicas e de filtração avançada.

## Approach

Mapeamento sistemático da relação entre a pressão do ar comprimido, a taxa de injeção da solução polimérica e a viscosidade do fluido, correlacionando-as com o diâmetro médio das fibras obtidas.

```ts
export const predictFiberMorphology = (pressurePsi: number, feedRateMlPerHour: number) => ({
  beadFormationRisk: feedRateMlPerHour > 5.0 && pressurePsi < 30,
  recommendedAction: 'Increase gas pressure to ensure complete solvent attenuation.'
});