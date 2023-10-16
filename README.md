# ﻿Previsão de Renda de Clientes


# Descrição do Projeto:
Este projeto visa prever a renda de clientes com base em variáveis sociodemográficas e econômicas. Utilizei técnicas de regressão linear e análise de dados para entender quais fatores mais influenciam na renda de um indivíduo.

# Características dos Dados:
Os dados contêm várias variáveis independentes que abrangem aspectos socioeconômicos, tais como:


data_ref	             
Data de referência de coleta das variáveis

index	                  
Código de identificação do cliente

sexo	                  
Sexo do cliente

posse_de_veiculo	      
Indica se o cliente possui veículo

posse_de_imovel	        
Indica se o cliente possui imóvel

qtd_filhos	            
Quantidade de filhos do cliente

tipo_renda	            
Tipo de renda do cliente

educacao	              
Grau de instrução do cliente

estado_civil	          
Estado civil do cliente

tipo_residencia	        
Tipo de residência do cliente (própria, alugada etc)

idade	                  
Idade do cliente

tempo_emprego	          
Tempo no emprego atual

qt_pessoas_residencia	  
Quantidade de pessoas que moram na residência

renda	                  
Renda em reais


# Ferramentas Utilizadas:
Python 3.x
Jupyter Notebook
Pandas
Numpy
Matplotlib
Statsmodels
Scikit-learn

# Instalação e Execução
Para rodar este projeto:

Clone o repositório.
Instale as bibliotecas necessárias.
Execute os notebooks Jupyter na ordem especificada.

# Metodologia:
Limpeza de Dados: Removemos valores nulos e outliers que poderiam distorcer os resultados.
Análise Exploratória: Utilizamos estatísticas e gráficos para entender melhor nossos dados.
Regressão Linear Simples: Começamos com um modelo simples usando apenas o tempo de emprego para prever a renda.
Regressão Linear Múltipla: Melhoramos nosso modelo incluindo mais variáveis.
Transformações e Ajustes: Testamos várias transformações matemáticas para melhorar ainda mais o modelo.

# Notebooks do Projeto
Regressão Linear Simples
Transformações em X e Y
Regressão Múltipla

# Resultados e Análise do Modelo
Nesta seção, detalhamos o processo de chegada ao nosso modelo final e as métricas de desempenho que consideramos.

# Regressão Linear Simples - Primeira Iteração
Começamos com uma abordagem de regressão linear simples, utilizando apenas o tempo de emprego como variável explicativa para prever a renda. O modelo resultante teve um R2 de 0.149, significando que apenas 14,9% da variação na renda poderia ser explicada pelo tempo de emprego. Embora isso tenha sido um bom ponto de partida, sabíamos que poderíamos fazer melhor.

# Regressão Linear Múltipla - Segunda Iteração
Na segunda iteração, incluímos múltiplas variáveis, como sexo, posse de veículo, tipo de renda, entre outras. Isso melhorou nosso R2 para 0.256, o que foi um passo significativo na direção certa. No entanto, a análise dos resíduos mostrou que ainda havia espaço para melhorias, principalmente porque os resíduos não estavam bem distribuídos em torno do zero.

# Transformações e Ajustes - Terceira Iteração
Para melhorar ainda mais o modelo, tentamos várias estratégias:

Transformações Logarítmicas: Ao aplicar a transformação logarítmica à variável de renda e tempo de emprego, conseguimos linearizar a relação entre as variáveis e melhorar o ajuste do modelo.

Interactions e Polinomiais: Adicionamos termos polinomiais e interações entre variáveis para capturar efeitos não-lineares e complexos entre as variáveis.

O modelo resultante após essas transformações mostrou um R2 ajustado de 0.35. Isso significa que nosso modelo final é capaz de explicar aproximadamente 35% da variação na renda dos clientes, o que é significativamente melhor do que nosso modelo inicial.

# Métricas de Desempenho 
R2Ajustado: 0.35
F-statistic: 172.1
P-value para variáveis significativas: < 0.05
Essas métricas indicam que o modelo é estatisticamente significativo e que as variáveis incluídas têm um efeito real sobre a variável de resposta, que é a renda.

# Análise de Resíduos
Depois de ajustar o modelo, é crucial analisar os resíduos (ou seja, a diferença entre os valores previstos e os valores reais) para validar a qualidade do ajuste. Em nosso modelo final, os resíduos estão bem distribuídos em torno do zero e não mostram padrões claros, o que é um bom sinal. Isso sugere que o modelo é robusto e faz um bom trabalho ao capturar a variabilidade na renda dos clientes.

# Aplicações Práticas

Avaliar a elegibilidade para diferentes tipos de empréstimos ou créditos.
Segmentar clientes para diferentes tipos de ofertas ou serviços.
Identificar clientes em potencial que possam estar interessados em novos produtos ou serviços.

# Licença
Este projeto está sob a licença MIT.
