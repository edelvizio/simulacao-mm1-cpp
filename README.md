# simulacao-mm1-cpp
Exemplo: simulação de eventos discretos em C++ (M/M/1)

1. Objetivo do experimento

Validar, por meio de simulação, o comportamento de um sistema de filas M/M/1, comparando:
resultados empíricos (simulados)
resultados analíticos (teóricos)
com foco nas métricas:
𝐿 (número médio no sistema)
𝐿𝑞	​ (número médio na fila)
𝑊 (tempo médio no sistema)
𝑊𝑞	(tempo médio na fila)

2. Hipóteses experimentais

H1 — Estabilidade do sistema
Se 𝜆<𝜇, então o sistema converge para regime estacionário.
H2 — Divergência próxima da saturação
À medida que 𝜌→1, as métricas 𝐿,𝐿𝑞,𝑊,𝑊𝑞​ crescem rapidamente.
H3 — Convergência estatística
Para valores altos de 𝑁, os resultados simulados aproximam-se dos valores teóricos.
H4 — Sensibilidade à taxa de chegada
Pequenas variações em 𝜆 próximas de 𝜇 geram grandes impactos nas métricas.

3. Planejamento experimental
Fixado inicialmente:
𝜇=𝟏.𝟎
𝑁=𝟏𝟎.𝟎𝟎𝟎
𝒔𝒆𝒆𝒅 = 𝟏𝟐𝟑𝟒𝟓

4. Coleta de dados
Registrar, para cada execução:
𝑳𝒔𝒊𝒎	​
𝑳𝒒,𝒔𝒊𝒎
​𝑾𝒔𝒊𝒎
​𝑾𝒒,𝒔𝒊𝒎

5. Cálculo dos valores teóricos
Para cada experimento, calcular:
𝑳𝒕𝒆𝒐	​
𝑳𝒒,𝒕𝒆𝒐
​𝑾𝒕𝒆𝒐
​𝑾𝒒,𝒕𝒆𝒐

6. Comparação quantitativa
Calcular o erro relativo:

𝑬𝒓𝒓𝒐 𝑹𝒆𝒍𝒂𝒕𝒊𝒗𝒐=|(〖𝑽𝒂𝒍𝒐𝒓〗_𝒔𝒊𝒎−〖𝑽𝒂𝒍𝒐𝒓〗_𝒕𝒆𝒐)/〖𝑽𝒂𝒍𝒐𝒓〗_𝒕𝒆𝒐 |

7. Perguntas a serem respondidas com os experimentos:
1) Ao executar: g++ src/main.cpp -o mm1 e ./mm1 0.9 1.0 10000 12345, o que acontece?
2) Os resultados simulados convergem para os teóricos?
3) Em quais condições o erro aumenta?
4) Qual o impacto da proximidade de 𝜆 e 𝜇?
5) O valor de 𝑁 foi suficiente?
6) Como a aleatoriedade influencia os resultados?

Respostas: somente serão aceitas aquelas enviadas pelo TEAMS (Modelagem Computacional)!
