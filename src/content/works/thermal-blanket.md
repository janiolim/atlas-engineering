---
title: "Controle Inteligente de Segurança para Manta Térmica"
description: "Circuito eletrônico microcontrolado focado no monitoramento térmico contínuo e prevenção de falhas catastróficas."
category: "engineering"
thumbnail: "./thermal-blanket.jpg"
tech:
  - Sistemas de controle
  - Segurança de Hardware
  - Termistores NTC
  - Arduino aplicado
order: 5
publishDate: 2026-07-04
---

## Brief

Dispositivos de aquecimento por contato direto apresentam riscos severos de queimadura ou incêndio em caso de falha no termostato convencional ou curto-circuito.

## Approach

Desenvolvimento de um sistema com redundância de sensores NTC dispersos na malha da manta, operando com um laço de controle que corta a alimentação principal via relé de estado sólido ao menor sinal de anomalia térmica.

```ts
export const verifyThermalSafety = (tempSensors: number[]) => {
  const maxAllowedTemp = 65; // em °C
  const hasOverheating = tempSensors.some(t => t > maxAllowedTemp);
  return {
    powerCutoff: hasOverheating,
    log: hasOverheating ? 'CRITICAL: Thermal runaway detected!' : 'Temperature within nominal bounds.'
  };
};