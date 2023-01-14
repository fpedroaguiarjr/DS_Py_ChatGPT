TESTE SHAPIRO-WILK (NORMALIDADE) POR ChatGPT

O teste de normalidade de Shapiro-Wilk é um teste estatístico que é utilizado para verificar se uma amostra de dados veio de uma distribuição normal. O teste é bastante preciso, mas exige um tamanho de amostra relativamente pequeno (geralmente n ≤ 2000). 
Gráfico da distribuição normal

Neste exemplo, geramos uma amostra de dados aleatórios de uma distribuição normal e, em seguida, executamos o teste de Shapiro-Wilk usando a função shapiro da biblioteca SciPy. O valor-p retornado pelo teste é comparado com um nível de significância alpha pré-determinado (neste caso, alpha = 0,05). Se o valor-p for maior que alpha, não podemos rejeitar a hipótese nula de que a amostra veio de uma distribuição normal; caso contrário, rejeitamos a hipótese nula e concluímos que a amostra não veio de uma distribuição normal.

Um dos melhores gráficos para verificar se uma distribuição é normal é o histograma, juntamente com uma sobreposição da curva normal teórica. Em Python, você pode usar a biblioteca "matplotlib" para criar um histograma e a biblioteca "scipy" para gerar a curva normal.
Para criar um histograma, você pode usar a função "plt.hist()" do matplotlib e especificar os dados, o número de barras (bins) e outras opções, como rótulos de eixo e títulos.
Para gerar a curva normal, você pode usar a função "scipy.stats.norm.pdf()", que gera os valores da função de densidade de probabilidade normal para uma determinada média e desvio padrão.
Este exemplo gera um histograma dos dados gerados aleatoriamente e sobrepõe a curva normal teórica. Ajustando os parâmetros de mu(População ) e std(Desvio padrão) para os dados, você pode comparar a distribuição dos dados com a curva normal e verificar se ela segue uma distribuição normal
