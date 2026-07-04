---
title: "Engenharia de Materiais para Armazenamento de Energia"
description: "Investigação da relação processamento-estrutura-desempenho em eletrodos avançados de supercapacitores e baterias."
category: "engineering"
thumbnail: "./energy-storage-materials.jpg"
tech:
  - materiais para energia
  - Eletroquímica
  - Supercapacitores
order: 9
publishDate: 2026-07-04
---

## Brief

O desenvolvimento de dispositivos de armazenamento de energia mais rápidos e eficientes passa pela compreensão fundamental de como a arquitetura do material afeta os mecanismos de difusão de íons e transferência de carga.

## Approach

Avaliação comparativa de diferentes arquiteturas baseadas em carbono, óxidos e hidróxidos metálicos submetidos a testes de carga/descarga galvânica contínua e espectroscopia de impedância eletroquímica.

```ts
export const analyzeEnergyDensity = (capacitance: number, voltageWindow: number) => ({
  specificEnergyWhKg: (0.5 * capacitance * Math.pow(voltageWindow, 2)) / 3.6,
  optimizationFocus: 'Expand voltage window stability to maximize power density.'
});