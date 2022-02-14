# All In - Segmentação de Clientes - Ciclo 2

A empresa All In é uma empresa de franquias Delicatesses. Delicatesse é uma loja que vende comidas finas e iguarias. Especializada em comidas exóticas, raras e de difícil preparo.
Os principais produtos da All In são vinhos, carnes, certos peixes, doces e guloseimas e o diferencial, você pode comprar certas peças de ouro.
<p align="center">
  <img src="https://portaldoqueijo.com.br/site/wp-content/uploads/2018/04/combina%C3%A7%C3%A3o-perfeita-queijos-e-vinhos.jpg">
</p>.

# Problema de Negócio

Após a primeira iteração do processo de segmentação de clientes, cujo objetivo era conhecer melhor a relação dos clientes com a empresa a fim de aumentar a retenção, a equipe de marketing esta buscando agora conhecer os hábitos de consumo dos clientes, para assim aumentar a taxa de conversão das campanhas com um marketing mais direto, além de adquirir conehcimento sobre como se conectar com cada cliente.

A franquia All In nos contratou para auxiliarmos a equipe de marketing em sua missão de melhorar a taxa de conversão.

# Solução Proposta

Uma maneira eficaz de descobrir padrões entre os hábitos de consumo de nossos clientes seria utilizar um algoritimo de clusterização. Um algoritimo de clusterização ira buscar semelhanças entre os hábitos de consumo dos clientes assim identificando agrupamentos naturais.

Podemos assim, analisar os agrupamentos naturais achados e seu comportamento, com essa análise a equipe de marketing irá saber aonde e como se conectar com certos clientes com um marketing direcionado e por consequêcia a taxa de conversão, a retenção e a interação irão aumentar.

# Modelagem

Para esta abordagem o algoritimo k-means foi escolhido. Utilizamos o gráfico de elbow para identificar o número ideal de cluster, que foi identificado como 3.

## Resultados da Segmentação

Possuímos 3 grupos bem equilibrados quanto ao número de clientes em cada um. Podemos ver no gráfico abaixo:

<p align="center">
  <img src="https://github.com/leorviana/segmentacao_de_clientes_2/blob/main/images/cluster_distribution.png">
</p>

Abaixo, utilizamos o modelo de redução de dimensionalidade **T-SNE** para conseguirmos visualizar os agrupamentos em 2D:

<p align="center">
  <img src="https://github.com/leorviana/segmentacao_de_clientes_2/blob/main/images/tsne_graph.png">
</p>

Podemos aqui visualizar como os agrupamentos estão um em relação ao outro e sua separação.

## Análise dos Agrupamentos

### Local de Compra X Grupos

<p align="center">
  <img src="https://github.com/leorviana/segmentacao_de_clientes_2/blob/main/images/local_compra.png">
</p>

1. Os 3 grupos criados compram mais ou menos igual pela internet, apesar de que o cluster 0 se sobressai.
2. Os clientes do cluster 2 compram bem mais pelo catálogo que os outros clientes.
3. Os clientes do cluster 1 costumam comprar mais na loja que os outros clientes, apesar de ser bem balanceado.

### Frequência e Gasto de Cada Grupo

<p align="left">
  <img src="https://github.com/leorviana/segmentacao_de_clientes_2/blob/main/images/frequencia_compras.png">
</p>

Os clientes do cluster 2 são os mais frequentes, seguidos do cluster 0 e por fim do cluster 1.

### Hábitos de Compra
Aqui, vamos olhar para os itens que cada grupo costuma comprar.

#### Cluster 0
<p align="left">
  <img src="https://github.com/leorviana/segmentacao_de_clientes_2/blob/main/images/itens_cluster_0.png">
</p>

- Clientes que amam vinho, mas compram muito pouco de qualquer outra mercadoria.

#### Cluster 1
<p align="left">
  <img src="https://github.com/leorviana/segmentacao_de_clientes_2/blob/main/images/itens_cluster_1.png">
</p>

- Possuem um padrão de compra mais regular, suas compras são diversificadas, bem mais que os outros grupos.

#### Cluster 2
<p align="left">
  <img src="https://github.com/leorviana/segmentacao_de_clientes_2/blob/main/images/itens_cluster_2.png">
</p>

- Clientes que compram bastante vinho e carne, mas muito pouco das outras mercadorias ainda.


## Concluindo a Análise

Podemos explicar os 3 agrupamentos naturais descobertos a partir das seguintes características:

**Cluster 0**: Clientes com uma frequência mediana que compram muito vinho, principalmente pela loja fisíca e pela internet.


**Cluster 1**: Clientes que compram poucas vezes, mas compram itens bem diversificados, compram em sua maioria na loja fisíca.


**Cluster 2**: São os clientes que mais compraram conosco, compram bastante vinho e bastante carne, compram significativamente mais pelo catálogo que outros clientes.

# Conclusão

Após todo o processo conseguimos identificar e analisar nossos clientes devidamente entre os 3 grupos naturais que eles se encontram divididos e agora somos capazes de se comunicar melhor com cada tipo de cliente e elevar os lucros, reduzir custos, reter melhor os clientes e gerir campanhas personalizadas.

# Referências

Laika. "Descubra o que é marketing direto e seus benefícios". **Blog Tiny**. Disponível em: <https://blog.tiny.com.br/gestao/marketing-direto/>.

GONG, Destin. "Clustering Algorithm for Customer Segmentation". **Towards Data Science**. Disponível em: <https://towardsdatascience.com/clustering-algorithm-for-customer-segmentation-e2d79e28cbc3>.
