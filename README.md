# Transfer Learning com ResNet50V2 - DIO

Este projeto é uma implementação de Transferência de Aprendizado utilizando o modelo **ResNet50V2** para classificar imagens de **gatos** e **cachorros**. A iniciativa faz parte de um estudo com a Digital Innovation One (DIO) e explora técnicas de aprendizado profundo.

---

## **Estrutura do Repositório**

- **`notebooks/`**
  - Contém o notebook Jupyter com o código de treinamento e avaliação do modelo: `transfer_Learning.ipynb`.
  
- **`images/`**
  - Imagens de teste para validação do modelo (`aisha.jpg` e `bob.jpg`).
  
- **`models/`** *(opcional)*
  - Modelos treinados salvos (se necessário para futuros carregamentos e inferências).

- **`data/`** *(opcional)*
  - Dataset utilizado no projeto.

---

## **Principais Funcionalidades**
- Pré-processamento de imagens para uso com o modelo ResNet50V2.
- Treinamento do modelo com Transfer Learning, usando o dataset de gatos e cachorros.
- Visualização do desempenho do modelo (gráficos de perda e acurácia).
- Classificação de novas imagens fornecidas pelo usuário.

---

## **Resultados**
Após 5 épocas de treinamento, o modelo alcançou os seguintes resultados:
- **Acurácia no treino:** 99,68%
- **Acurácia na validação:** 98,47%

Gráficos de desempenho são gerados para acompanhar a evolução da perda e acurácia durante o treinamento.

---

## **Requisitos**

Certifique-se de que você tem as seguintes dependências instaladas:

- Python 3.x
- TensorFlow
- NumPy
- Matplotlib
- Pillow

Para instalar, execute:

```bash
pip install tensorflow numpy matplotlib pillow
```

---

## **Como Usar**

## 1. Clonar o Repositório

Clone o projeto para sua máquina local:

```bash
git clone https://github.com/eunafita/transfer-learning-dio.git
```

## 2. Estrutura do Projeto

Certifique-se de que a estrutura esteja semelhante a esta:

```arduino
transfer-learning-dio/
├── notebooks/
│   └── transfer_Learning.ipynb
├── images/
│   ├── aisha.jpg
│   └── bob.jpg
├── models/
├── data/
└── README.md
```

# **3. Executar o Notebook**

1. Abra o arquivo notebooks/transfer_Learning.ipynb no Jupyter Notebook ou Google Colab.
1. Siga as instruções do notebook para:
Treinar o modelo com Transfer Learning.
Fazer previsões com novas imagens.

---

## **Exemplo de Uso**

No notebook, você pode testar imagens fornecendo o caminho para o arquivo de imagem. Por exemplo:

```python
# Caminho para a imagem externa
image_path = "./images/aisha.jpg"

# Fazer a previsão
predicted_class = "Gato" if predicted_prob > 0.5 else "Cachorro"
print(f"Predição: {predicted_class}")
```

Resultado esperado:
Para aisha.jpg (cachorro), o modelo deve retornar "Cachorro".
Para bob.jpg (gato), o modelo deve retornar "Gato".

---

## **Customizações Futuras**

Adicionar mais classes ao modelo.
Implementar uma interface gráfica para upload de imagens.
Salvar o modelo treinado e disponibilizar para uso em produção.

## **Autor**

Este projeto foi desenvolvido por Rafael Danilo Santos Bortoluzzi.

Se você gostou deste projeto, não esqueça de deixar uma ⭐ no repositório!













