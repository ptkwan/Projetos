# 🎲 Projeto Final – Lógica de Programação 1 com Python  
**Ada Tech & iFood**

---

## 📌 Sumário

- [💡 Definição do Problema](#-definição-do-problema)  
- [🌟 As Recomendações](#-as-recomendações)  
- [👥 Integrantes](#-integrantes)  
- [🤔 O que é o KNN?](#-o-que-é-o-knn)  
- [⚙️ O Desenvolvimento](#️-o-desenvolvimento)  
  - 1️⃣ Executando os conjuntos de dados  
  - 2️⃣ Função `distancia_euclidiana`  
  - 3️⃣ Tratamento de Empates  
  - 4️⃣ Cálculo das Distâncias  
  - 5️⃣ Classificação por CPF  
  - 6️⃣ Novas Classificações  
- [✅ Conclusão](#-conclusão)  
- [🔗 Links Úteis](#-links-úteis)

---

## 💡 Definição do Problema

Recebemos um conjunto de dados contendo:

- CPF do cliente (`int`)  
- Classificação NPS (`string`: *Promotor, Neutro ou Detrator*)  
- Valores das 4 últimas compras (`tupla` com `float`)

Nosso objetivo foi prever a **classificação NPS** de novos clientes (ainda não classificados), com base no comportamento de clientes anteriores, utilizando o algoritmo **KNN (K-Nearest Neighbors)**.

Essa análise visa **melhorar o atendimento personalizado**, prevendo a satisfação de novos clientes.

---

## 🌟 As Recomendações

Regras do projeto:
- Uso apenas de **funções próprias e built-in** do Python  
- Utilização de **listas**, **tuplas**, **condições** e **laços de repetição**  
- Nada de bibliotecas externas

---

## 👥 Integrantes

- Alan Gonçalves  
- Élen Silva Almeida  
- Gabriel Matina  
- Gustavo Dell Anhol Oliveira  
- Patrick Kwan  

---

## 🤔 O que é o KNN?

O algoritmo **KNN** (K-Nearest Neighbors) é um dos primeiros métodos aprendidos em Machine Learning. Ele classifica uma amostra analisando seus vizinhos mais próximos com base em **distância** (neste projeto, a distância **Euclidiana**).

> Se a maioria dos 5 vizinhos mais próximos for "Promotor", o novo cliente será classificado como Promotor.

Valor de `K` utilizado: **5**
