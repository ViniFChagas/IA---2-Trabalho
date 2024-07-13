# IA - 2º Trabalho - Raciocínio Probabilistico

Docente: Edjard Mota
Discente: Vinicius Chagas (22050485)

Trabalho avaliativo da disciplina de Inteligência Artificial, ministrada pelo professor Edjard Mota.


## Introdução

As redes bayesianas são ferramentas poderosas para modelar e raciocinar sobre sistemas complexos com variáveis incertas. Ao representar as relações entre os diversos componentes do sistema como uma rede de nós interconectados, as redes bayesianas podem calcular de forma eficiente a probabilidade de diferentes resultados, dadas as evidências observadas.


Nesse trabalho, será feito um sistema de diagnóstico para um farol de bicicleta movido a dínamo, usando uma rede bayesiana. As variáveis são fornecidas na tabela abaixo:


![tabela variáveis](https://github.com/user-attachments/assets/a285f223-1b28-46a6-a049-faff6d474c6a)


As seguintes variáveis são independentes aos pares: Str, Flw, B, K. Além disso: (R, B), (R, K), (V, B), (V, K) são independentes e a seguinte equação é válida:


P(Li | V, R) = P(Li | V)
P(V | R, Str) = P(V | R)
P(V | R, Flw) = P(V | R)


Além disso temos a seguinte tabela comparando as influências que as variáveis V, B e K têm em P(Li):


![tabela P(Li)](https://github.com/user-attachments/assets/c82ebf07-78b6-41f3-a828-678754937e00)


Foi feito também uma rede causalidade entre as variáveis Str, Flw, R, V, B, K e Li:


![rede causalidade completa](https://github.com/user-attachments/assets/413f501d-6df7-4c92-b4b2-09b8a654a3e7)



## Objetivo


Com base na rede causalidade criada, será implementado o problema em questão em ProLog e também será mostrado a solução para P(V | Str = snow_covered).



## Referências
 
https://dtai.cs.kuleuven.be/problog/tutorial/basic/02_bayes.html


