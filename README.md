# 🌱 Edge AI para Detecção de Estresse Hídrico e Pragas com Redução de Overhead de Rede

> Projeto da disciplina de Inteligência Artificial — Universidade Presbiteriana Mackenzie  
> Faculdade de Computação e Informática — 7º Período CC Noite  
> Prof. Dr. Ivan Carlos Alcântara de Oliveira

---

## 👥 Integrantes

| Nome | RA | E-mail |
|------|----|--------|
| Gabriel Vieira de Sousa | 10410264 | 10410264@mackenzista.com.br |
| Guilherme Rainho Geraldo | 10418251 | 10418251@mackenzista.com.br |
| Guilherme Gomes Arantes Teles | 10364065 | 10364065@mackenzista.com.br |

---

## 📋 Descrição do Projeto

Sistema de **visão computacional embarcado em dispositivos de borda** (Raspberry Pi 4) para identificar, em tempo real, sintomas de **estresse hídrico** e **presença de pragas** em folhas de plantações.

O sistema utiliza modelos de Deep Learning otimizados com **TensorFlow Lite** e transmite apenas alertas via protocolos de comunicação eficientes (**LoRaWAN / MQTT**), reduzindo o overhead de rede em até **90%** em comparação com abordagens tradicionais baseadas em nuvem.

**Área:** Sustentabilidade / Agricultura / Redes  
**Opção:** ML/DL/VC/PLN (Visão Computacional + Deep Learning)

---

## 🗂️ Estrutura do Repositório

```
edge-ai-plant-disease/
│
├── README.md                  # Este arquivo
│
├── docs/
│   └── Artigo_N1_EdgeAI.docx  # Relatório parcial (formato SBC)
│
├── dataset/
│   └── README.md              # Descrição e instruções do dataset
│
└── notebooks/
    └── 01_analise_exploratoria.ipynb  # Análise exploratória do PlantVillage
```

---

## 🛠️ Tecnologias Utilizadas

- Python 3.10+
- TensorFlow / TensorFlow Lite
- MobileNetV2
- OpenCV
- Pandas, NumPy, Matplotlib, Seaborn
- Jupyter Notebook

---

## 📊 Dataset

Utilizamos o dataset **PlantVillage** — 54.305 imagens de folhas de plantas, organizadas em 38 classes (14 espécies × 26 doenças + folhas saudáveis).

Detalhes em [`dataset/README.md`](dataset/README.md).

---

## 📄 Relatório

O artigo parcial (Parte 2 - N1) está disponível em [`docs/`](docs/) no formato do template SBC fornecido pelo professor.

---

## 📅 Histórico de Atualizações

| Data | Autor | Descrição |
|------|-------|-----------|
| 22/05/2026 | Guilherme Teles | Criação do repositório e estrutura inicial |
| 22/05/2026 | Guilherme Teles | Adição do notebook de análise exploratória |
| 22/05/2026 | Guilherme Teles | Adição do relatório N1 e descrição do dataset |
