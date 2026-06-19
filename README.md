#  Classificação de Imagens: Gatos e Cachorros

##  Sobre o projeto

Este projeto foi desenvolvido para a disciplina de **Inteligência Artificial** do curso de **Ciência da Computação**.

O objetivo é desenvolver diferentes abordagens utilizando **Redes Neurais Artificiais** para realizar a classificação de imagens de cães e gatos.

O trabalho compara três técnicas:

1. **MLP (Multilayer Perceptron) implementada manualmente**
2. **CNN (Convolutional Neural Network) utilizando PyTorch**
3. **CNN com Transfer Learning utilizando modelos pré-treinados**

---

#  Objetivos

O projeto tem como objetivo compreender diferentes níveis de implementação de Redes Neurais Artificiais:

- Entender os fundamentos matemáticos das redes neurais
- Implementar algoritmos de aprendizado manualmente
- Utilizar frameworks modernos de Deep Learning
- Aplicar modelos pré-treinados para classificação de imagens

---

#  Abordagens implementadas

##  MLP - Rede Neural Multicamadas (Manual)

Nesta etapa foi desenvolvida uma rede neural do zero utilizando apenas bibliotecas básicas.

### Pré-processamento:

- Redimensionamento das imagens para:

```
64x64 pixels
```

- Conversão para tons de cinza
- Transformação das imagens em vetores

### Implementações realizadas:

✅ Forward Propagation  
✅ Função de ativação ReLU  
✅ Função Sigmoid  
✅ Binary Cross Entropy  
✅ Backpropagation  
✅ Gradiente Descendente  

### Arquitetura:

```
Entrada:
4096 neurônios

Camada oculta:
128 neurônios + ReLU

Saída:
1 neurônio + Sigmoid
```

---

# 2️⃣ CNN - Rede Convolucional com PyTorch

Nesta etapa foi desenvolvida uma rede neural convolucional utilizando:

- PyTorch
- TorchVision

A CNN utiliza imagens coloridas em:

```
3 x 224 x 224
```

### Componentes utilizados:

- Camadas convolucionais
- Pooling
- Camadas totalmente conectadas
- Data Augmentation

### Técnicas de aumento de dados:

- Rotação
- Espelhamento
- Alteração de brilho/contraste

---

# 3️⃣ Transfer Learning

Nesta etapa foram utilizados modelos pré-treinados disponíveis no TorchVision.

O objetivo é adaptar redes já treinadas para o problema de classificação de cães e gatos.

Modelos utilizados:

- ResNet
- MobileNet
- VGG
- AlexNet

### Alterações realizadas:

- Adaptação das camadas finais
- Fine-tuning
- Treinamento para nova tarefa

---

# 📂 Estrutura do projeto

```
projeto/
│
├── data/
│   └── train/
│       ├── cat/
│       └── dog/
│
├── MLP/
│   └── mlp_manual.ipynb
│
├── CNN/
│   └── cnn_pytorch.ipynb
│
├── TransferLearning/
│   └── transfer_learning.ipynb
│
├── requirements.txt
│
└── README.md
```

---

# ⚙️ Tecnologias utilizadas

## Linguagem

- Python

## Bibliotecas

- NumPy
- Matplotlib
- Pillow
- Pandas
- PyTorch
- TorchVision

---

# 📦 Instalação

Clone o repositório:

```bash
git clone <url-do-repositorio>
```

Entre na pasta:

```bash
cd projeto
```

Instale as dependências:

```bash
pip install -r requirements.txt
```

---

#  Execução

Execute os notebooks na ordem:

## MLP

```bash
jupyter notebook MLP/mlp_manual.ipynb
```

## CNN

```bash
jupyter notebook CNN/cnn_pytorch.ipynb
```

## Transfer Learning

```bash
jupyter notebook TransferLearning/transfer_learning.ipynb
```

---

# 📊 Avaliação

Os modelos são avaliados utilizando:

- Acurácia
- Loss
- Tempo de treinamento
- Matriz de confusão

Os resultados são comparados considerando:

- Facilidade de implementação
- Custo computacional
- Desempenho
- Aplicabilidade prática

---

#  Comparação esperada

| Modelo | Característica |
|---|---|
| MLP | Implementação simples, porém limitada para imagens |
| CNN | Melhor aproveitamento de características visuais |
| Transfer Learning | Melhor desempenho utilizando conhecimento prévio |

---
