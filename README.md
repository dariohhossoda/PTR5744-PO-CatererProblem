# PTR5744 - Pesquisa Operacional Aplicada ao Planejamento de Transportes (2022)

## O Problema dos Guardanapos (The Napkin Problem)

### Introdução
Este repositório é um exercício visto em sala de aula da disciplina PTR5744 - Pesquisa Operacional Aplicada ao Planejamento de Transportes de 2022, ministrado pelo professor Claudio Barbieri da Cunha. O intuito deste trabalho é o estudo e aplicação de problemas de fluxo em rede, sendo o exemplo descrito a seguir um caso particular de aplicação desta problemática.


O problema dos guardanapos é um tipo de problema do fornecedor (The Caterer Problem), em que um fornecedor deve providenciar guardanapos limpos durante um período de $\color{grey}n$ dias; o número de $\color{grey}d_j$ guardanapos requiridos no dia $\color{grey}j$ já é conhecido. Para satisfazer esses requisitos, o fornecedor pode tanto comprar novos guardanapos (por $\color{grey}a$ centavos/peça) ou ter os guardanapos usados lavados. A lavanderia providencia um serviço rápido (guardanapos retornam $\color{grey}q$ dias depois por um preço $\color{grey}b$ centavos/peça) e um serviço lento (guardanapos são devolvidos $\color{grey}p$ dias depois por um preço $\color{grey}c$ centavos/peça).

Naturalmente, $\color{grey}p>q$  e  $\color{grey}a>b>c$. Para ilustração, será considerado o caso de $\color{grey}n=10$, $\color{grey}\\ d_1=50, \ d_2=60, \ d_3=80, \ d_4=70, \ d_5=50,\\ d_6=60,\ d_7=90,\ d_8=80,\ d_9=50, \ d_{10}=100$

 e

 $\color{grey}p=4, \ q=2; \ a=200, \  b=75, \ c=25$.

### Estrutura da Rede
<p align="center">
    <img src="https://user-images.githubusercontent.com/58784697/170809989-f813493c-0a63-4add-9f6a-348d1550af2b.svg" alt="EstruturaRede" style="width:250px;"/>
</p>

#### Significado da rede

Os nós centrais representam hierarquicamente os guardanapos requiridos a cada dia, ao passo que os nós da esquerda são provenientes da lavagem destes. Os arcos em <span style="color:red">vermelho</span> representam a compra de novos guardanapos, os arcos em <span style="color:green">verde</span> são provenientes da lavagem rápida e os arcos em <span style="color:#085CFC">azul</span>, da lavagem mais demorada.

### Modelagem do problema e resolução

Foi escolhida a modelagem e programação do problema a partir de um caderno Jupyter ([Jupyter Notebook](napkins.ipynb)) que pode ser visualizado no repositório por questões de praticidade e afinidade com a linguagem Python 3. Sendo a função objetivo o mínimo custo de fluxo na rede.

### Resultado do programa

Executando o _script_ de fluxo de custo mínimo pode-se obter a rede ótima.

<p align="center">
    <img src="https://user-images.githubusercontent.com/58784697/170810419-10b97bd7-a644-4915-826c-4b4563f6e053.svg" alt="EstruturaRede" style="width:250px;"/>
</p>

### Contato

#### Dário Hachisu Hossoda

Mestrando em Engenharia Hidráulica - POLI-USP

e-mail: dario.hossoda@usp.br
