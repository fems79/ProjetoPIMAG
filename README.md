# Detecção de Jogadores em Imagens de Futebol

## Descrição

Este projeto implementa um sistema de detecção de jogadores em imagens de partidas de futebol utilizando técnicas de Processamento Digital de Imagens.

A abordagem consiste em:

* Conversão do espaço de cores RGB para HSV
* Segmentação do campo por limiarização de cor
* Binarização dos objetos de interesse
* Operações de morfologia matemática (erosão e dilatação)
* Rotulagem de componentes conexos (Flood Fill)
* Filtragem por características geométricas
* Desenho de bounding boxes sobre os objetos detectados

---

## Estrutura do Repositório

```
.
├── notebooks/
│   └── deteccao_jogadores.ipynb
├── data/
│   └── imagens/
│       └── IMG-20260209-WA0013.jpg
├── resultados/
│   └── resultado_exemplo.png
├── apresentacao.md
└── README.md
```

* **notebooks/**: código da solução em Jupyter Notebook
* **data/**: imagens utilizadas nos experimentos
* **resultados/**: imagens geradas pelo algoritmo

---

## Como Executar

### Opção 1 – Google Colab

Abra o notebook diretamente no Colab:

(cole aqui o link do Colab)

Certifique-se de que o caminho da imagem está definido como:

```python
arquivo_imagem = 'data/imagens/IMG-20260209-WA0013.jpg'
```

---

### Opção 2 – Localmente

Instale as dependências:

```bash
pip install numpy matplotlib scikit-image
```

Execute o notebook:

```
notebooks/deteccao_jogadores.ipynb
```

---

## Técnicas Utilizadas

* Operações pixel a pixel
* Binarização
* Modelo de cores HSV
* Morfologia matemática binária

  * Erosão
  * Dilatação
  * Abertura e fechamento
* Segmentação por cor
* Rotulagem de componentes conexos
* Análise geométrica de regiões

---

## Resultados

O sistema é capaz de:

* Remover o campo (segmentação do verde)
* Detectar jogadores e bola
* Gerar bounding boxes sobre os elementos de interesse

---

## Vídeo de Apresentação

Link do YouTube (máx. 15 min):

[Coloque aqui o link]

---

## Autor

Nome do aluno
Disciplina: Processamento de Imagens
Ano: 2026
