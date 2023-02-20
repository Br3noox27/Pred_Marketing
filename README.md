 # Projeto - Previsão de sucesso de campanhas de marketing

[https://www.kaggle.com/loveall/clicks-conversion-tracking](https://www.kaggle.com/loveall/clicks-conversion-tracking)

# Descrição do problema

A empresa XYZ é uma grande empresa de streaming de vídeo e está enfrentando um alto índice de cancelamento de assinaturas. Eles coletaram dados dos usuários, incluindo informações sobre o uso do serviço, a taxa de assinatura e a satisfação do cliente. Neste problema, você pode usar um conjunto de dados do Kaggle que contém informações sobre anúncios on-line de uma empresa. O conjunto de dados contém informações sobre o anúncio, o site em que o anúncio foi exibido, o horário em que o anúncio foi exibido e a ação do usuário em relação ao anúncio (clique ou conversão). Você pode treinar um modelo de classificação usando esses recursos para prever se um usuário irá clicar ou converter em um anúncio e avaliar o desempenho do modelo usando métricas como precisão, recall e F1-score. A empresa pode usar esse modelo para segmentar seus usuários de acordo com a probabilidade de clicar ou converter em um anúncio e direcionar seus recursos de publicidade de maneira mais eficiente.

## *Tabela Variável*

Esta tabela contém informações sobre as variáveis presentes no conjunto de dados.

| Nome da Variável | Descrição da Variável |
| --- | --- |
| ad_id | O ID do anúncio |
| xyz_campaign_id | O ID da campanha de publicidade |
| fb_campaign_id | O ID da campanha de publicidade no Facebook |
| age | A idade do usuário que visualizou o anúncio |
| gender | O gênero do usuário que visualizou o anúncio |
| interest | O código de interesse do usuário (mais de um código é possível) |
| Impressions | O número de vezes que o anúncio foi exibido |
| Clicks | O número de vezes que o anúncio foi clicado |
| Spent | O valor gasto na exibição do anúncio |
| Total_Conversion | O número de conversões após a visualização do anúncio |
| Approved_Conversion | O número de conversões após a aprovação do anúncio |

# Explicação da variável resposta

No conjunto de dados "Clicks Conversion Tracking", as variáveis "Total_Conversion" e "Approved_Conversion" representam o número de conversões que ocorreram após a visualização e aprovação do anúncio, respectivamente. Portanto, dependendo do objetivo da análise, você pode escolher uma dessas variáveis como sua variável resposta. Por exemplo, se você estiver interessado em prever quantas conversões ocorrerão após a visualização do anúncio, "Total_Conversion" seria sua variável resposta. Se você estiver interessado em prever quantas conversões ocorrerão após a aprovação do anúncio, "Approved_Conversion" seria sua variável resposta.


# Ciclo 2

Neste ciclo, foram analisados os dados de serviço e informações do usuário.

Dados de Serviço:
Algo interessante que no marketing não tem apenas a maioria de vendas para um gênero de publico alvo, são bem compativel os dois e equivale ao mesmo.
A maioria do clientes o publico alvo a idade é em média dos 30 aos 34.
Ao porcentos dos clicks depois de ver os anúncios, os homens acabam saindo da frente das mulheres, então produtos masculinos chama mais atenção dos homens ao clicar.

O foco do projeto foi mais na realização de aprovação ao clicks e o caminho aonde chegar até aprovação, então,  fiz diversos gráficos demosntrando as idades com clicks, com aprovação e os totais de conversões.

o que podemos tirar desses gráficos tirando essas informações pessoas ? 

podemos ver que quanto mais colocarmos dinheiro ao ads o propósito é alcançar mais pessoas e deixar seus anúncios com mais visibilidade onde você quer (região, lugar etc). Porém, esse dinheiro, não transforma em mais dinheiro para você, coisa que era para acontecer, e todo mundo acha.

vemos que pessoas que pagam mais, mostram para muitas pessoas sim e também obtem mais clicks, porém, isso não transforma em aprovação e nem totais de conversão para eles que nisso, acaba não lucrando muito.

podemos tirar de conclusão, que temos que fazer um anúncio muito bem feito, igual uma mulher que vimos no gráfico, onde ela pagou menos de 2$ e chegou a ter 11% de aprovação isso sem tirar muito do seu bolso, mas claro, se gastarmos mais e fazermos um anúncio bem feito, nós podemos lucrar muito, igual o que mais teve aprovação, onde 40 pessoas foi o total de conversão e 21 de aprovação.

# ciclo 3 

para concluir o processo, observei as precisões: 
cross_val_score : 58% de precisão
KNN: obteve 62% de precisão.

Taxa de rotatividade antes do modelo: 276.42% e apos os modelos obtivemos esses resultados:

XGBoost reduziu para 150.66%.


KNN reduziu para 125.76% o menor até agora.

