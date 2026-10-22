# Dashboard Restelo T4 — Orçamento

Apresentação / dashboard interativo da **Proposta de Remodelação Restelo T4** (Imperiou's Remodelações):
Entrada, Cozinha, Lavandaria e 3 Casas de Banho — com todo o texto e imagens da proposta.

- Abrir: `index.html` (publicado via GitHub Pages pelo workflow `.github/workflows/pages.yml`).
- Interatividade: planta com zonas clicáveis, pontos interativos na cozinha / equipamentos / casa de banho,
  matriz de intervenção filtrável com gráficos, simulador de IVA, passos marcáveis, galeria dos 13 diapositivos
  originais e modo apresentação (botão ▶, setas ← →).
- Funciona offline (Chart.js incluído em `vendor/`).
- Imagens: `python3 tools/crop.py <pptx-extraído>/ppt/media assets` recorta-as a partir do PPTX.
