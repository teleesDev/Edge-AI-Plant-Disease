# 📦 Dataset — PlantVillage

## Descrição

O **PlantVillage Dataset** é uma coleção de referência amplamente utilizada na literatura para detecção de doenças em plantas via visão computacional.

| Atributo | Valor |
|----------|-------|
| Total de imagens | 54.305 |
| Número de classes | 38 |
| Espécies de plantas | 14 |
| Doenças cobertas | 26 |
| Resolução | 256 × 256 pixels |
| Formato | JPG |
| Licença | Creative Commons Attribution 4.0 (CC BY 4.0) |

## Origem

- **GitHub oficial:** https://github.com/spMohanty/PlantVillage-Dataset  
- **Kaggle:** https://www.kaggle.com/datasets/abdallahalidev/plantvillage-dataset  
- **Referência:** Hughes, D.; Salathé, M. *An open access repository of images on plant health to enable the development of mobile disease diagnostics.* arXiv:1511.08060, 2015.

## Classes Disponíveis

O dataset cobre as seguintes combinações espécie/condição (exemplos):

| Espécie | Condição |
|---------|----------|
| Apple | Apple Scab, Black Rot, Cedar Apple Rust, Healthy |
| Corn | Cercospora Leaf Spot, Common Rust, Northern Leaf Blight, Healthy |
| Grape | Black Rot, Esca, Leaf Blight, Healthy |
| Potato | Early Blight, Late Blight, Healthy |
| Tomato | Bacterial Spot, Early Blight, Late Blight, Leaf Mold, Mosaic Virus, Yellow Leaf Curl Virus, Healthy |
| ... | ... (38 classes no total) |

## Como Obter o Dataset

O dataset **não está incluído neste repositório** devido ao tamanho (~1,2 GB). Para reproduzir os experimentos:

```bash
# Opção 1: Kaggle CLI
pip install kaggle
kaggle datasets download -d abdallahalidev/plantvillage-dataset
unzip plantvillage-dataset.zip -d dataset/plantvillage/

# Opção 2: Download manual
# Acesse https://www.kaggle.com/datasets/abdallahalidev/plantvillage-dataset
# e faça o download manualmente para a pasta dataset/plantvillage/
```

## Estrutura Esperada

Após o download, a pasta deve ter a seguinte estrutura:

```
dataset/
├── README.md         ← este arquivo
└── plantvillage/
    ├── Apple___Apple_scab/
    │   ├── image001.jpg
    │   └── ...
    ├── Apple___Black_rot/
    ├── Tomato___Late_blight/
    └── ... (38 pastas no total)
```

## Pré-processamento Aplicado

- Redimensionamento para **224 × 224 pixels** (entrada do MobileNetV2)
- Normalização: pixels / 255.0 (escala [0, 1])
- Divisão: **70% treino / 15% validação / 15% teste**
- Data augmentation (apenas no treino): rotação ±30°, flip horizontal/vertical, zoom ±20%, ajuste de brilho/contraste

## Histórico de Atualizações

| Data | Autor | Descrição |
|------|-------|-----------|
| 10/05/2026 | Gabriel Vieira | Criação da descrição do dataset |
