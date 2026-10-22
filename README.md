# Dashboard Restelo T4 — Orçamento

Apresentação / dashboard interativo da **Proposta de Remodelação Restelo T4** (Imperiou's Remodelações):
Entrada, Cozinha, Lavandaria e 3 Casas de Banho — com todo o texto e imagens da proposta.

- Abrir: `index.html` (publicado via GitHub Pages pelo workflow `.github/workflows/pages.yml`).
- Interatividade: planta com zonas clicáveis, pontos interativos na cozinha / equipamentos / casa de banho,
  matriz de intervenção filtrável com gráficos, simulador de IVA, passos marcáveis, galeria dos 13 diapositivos
  originais e modo apresentação (botão ▶, setas ← →).
- Funciona offline (Chart.js incluído em `vendor/`).
- Planta 3D: `plan3d.js` desenha em SVG a planta (layout da Planta_Casa_1) com as 7 divisões intervencionadas
  (Entrada, Cozinha, Lavandaria e 4 casas de banho) e setas para cada uma.
- Imagens: `node tools/render_plan.js` gera `tools/plan3d.png` e `python3 tools/crop.py <pptx-extraído>/ppt/media assets`
  recorta os diapositivos do PPTX, aplicando as correções de `tools/patch_slides.py` (valores e planta 3D no diapositivo 2).
