---
title: "Projeto e Simulação de Sensor de Microfita em U"
description: "Modelamento eletromagnético e dimensionamento de ressoador em formato U sobre substrato FR-4 para radiofrequência."
category: "engineering"
thumbnail: "./u-microstrip.jpg"
tech:
  - Radiofrequência
  - Eletromagnetismo
  - Simulação Computacional
order: 4
publishDate: 2026-07-04
---

## Brief

Aplicações modernas de detecção e comunicação sem fio necessitam de sensores compactos, de baixo custo e com alta sensibilidade a variações de permissividade dielétrica do meio.

## Approach

Dimensionamento analítico das linhas de transmissão em formato 'U' acopladas eletromagneticamente, seguido de simulação numérica de parâmetros $S_{11}$ e $S_{21}$ em substrato FR-4 ($\varepsilon_r \approx 4.4$).

```ts
export const calculateResonantFrequency = (lengthMm: number, effectiveDielectric: number) => {
  const c = 3e8; // velocidade da luz
  return c / (2 * lengthMm * Math.sqrt(effectiveDielectric));
};