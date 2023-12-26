# modelos_regressao_avancada

## 1.Conjunto de Dados:

* Tamanho do conjunto de treinamento: 11.250
* Tamanho do conjunto de teste: 3.750
* Colunas do conjunto de features: posse_de_veiculo, posse_de_imovel, qtd_filhos, tipo_renda, educacao, tempo_emprego, qt_pessoas_residencia, renda
## 2. Regularização Ridge:

* Foram testados diferentes valores de alpha.
* O melhor modelo Ridge foi encontrado com alpha = 0, apresentando R2 de 1.0 e RMSE muito próximo de zero.
* Os coeficientes do melhor modelo indicam a influência de cada feature.
## 3. Regularização LASSO:

* Similar ao Ridge, testou-se diferentes valores de alpha.
* O melhor modelo LASSO foi encontrado com alpha = 0, também apresentando R2 de 1.0 e RMSE muito próximo de zero.
* Os coeficientes indicam a influência das features, com algumas delas recebendo peso zero (seleção de variáveis).
## 4. Modelo Stepwise:

* Foi aplicado um modelo stepwise na base de teste, resultando em R2 de 1.0 e RMSE próximo de zero.
## 5. Avaliação após Remoção de Outliers:

* Estatísticas da variável alvo (renda) antes e depois da remoção de outliers foram exibidas.
## 6. Ajuste de Modelos de Regressão Linear:

* Foram ajustados modelos Ridge e LASSO após a remoção de outliers.
* O aviso "SettingWithCopyWarning" foi gerado, sugerindo alteração para evitar o aviso.
## 7. Árvore de Regressão:

* Uma árvore de regressão foi ajustada, resultando em um R2 de aproximadamente 0.20.
## 8. Transformações Polinomiais:

* Foram aplicadas transformações polinomiais, mas um problema com valores NaN impediu o ajuste do modelo.
## 9. Avaliação do Log(Renda):

* A mediana e média do log(renda) foram avaliadas nos conjuntos de treinamento e teste.
## 10. Avaliação da Renda após Exponenciação:

* A mediana da renda foi calculada após exponenciar os valores do log(renda).

## 11. Agrupamento e Estatísticas:

* A renda foi dividida em 10 grupos e calculadas média, mediana, percentil 5% e percentil 95% para cada grupo.
Um gráfico foi gerado para visualizar essas estatísticas.

**Em resumo,** os modelos ajustados, incluindo Ridge, LASSO, árvore de regressão e stepwise, apresentaram um desempenho excepcional com um R2 próximo de 1.0 e RMSE próximo de zero. O aviso "SettingWithCopyWarning" indica uma possível melhoria no código para evitar problemas. A avaliação de modelos alternativos, como árvores de decisão, transformações polinomiais e agrupamento de renda, complementa a análise do desempenho dos modelos.
