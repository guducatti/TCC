# TCC — Produtividade da soja, NDVI e clima nos municípios brasileiros

Trabalho de Conclusão de Curso de Gustavo Ducatti: estimação e previsão da produtividade municipal da soja (IBGE/PAM) com NDVI (MODIS), temperatura (ERA5) e precipitação (CHIRPS), usando formas funcionais flexíveis de Fourier.

Este repositório guarda a versão original do trabalho. O artigo derivado dele está em um repositório próprio.

## Conteúdo

| Caminho | Descrição |
|---|---|
| `Monografia - Gustavo Ducatti.pdf` | Texto da monografia |
| `Apresentacao.pptx` | Apresentação da defesa |
| `# BASE MUNICIPAL.ipynb` | Scripts de agregação municipal dos dados em grade (CHIRPS) |
| `data_construction.ipynb` | Seleção dos municípios e construção da base |
| `data_validation.ipynb` | Validação do NDVI, da precipitação e da temperatura (inclui comparação com estações do INMET) |
| `model.ipynb` | Modelos em painel, avaliação fora da amostra e previsão |
| `Bases/` | Bases finais por período (`range(*)_final_data.csv`), malhas (`municipios_em_uso.*`, `BR_Pais_2024/`), dados do IBGE e do INMET |
| `Figuras/` | Figuras da monografia |
| `data_soja_PR.csv` | Recorte do Paraná |

Alguns notebooks têm caminhos absolutos da máquina onde foram executados; para rodar, ajuste-os para a pasta `Bases/` deste repositório.

## Fontes dos dados

- IBGE — Produção Agrícola Municipal (Tabela 5457) e malhas territoriais 2024.
- NASA — MODIS (NDVI).
- ECMWF/Copernicus — ERA5 (temperatura).
- UCSB/CHC — CHIRPS (precipitação).
- INMET — estações automáticas (validação).
