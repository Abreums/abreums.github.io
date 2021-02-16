## Uma análise sobre o batch size para projetos de TI

**Resumo:** entre os muitos conceitos Lean que migraram para as práticas ágeis em TI, um dos menos entendidos é o _batch size_ e de como ele pode ser gerenciado. neste artigo vamos apresentar alguns conceitos e análise sobre o tema.

### 1. O Batch Size como componente do Custo

Para entender _batch size_ imagine uma linha de produção capaz de produzir 2 produtos diferentes: A e B. O tempo de produção de ambos é igual - 1 unidade de tempo por unidade de produto. Porém, para mudar a produção de um produto para outro é preciso ajustar a linha e este tempo de _setup_ toma 2 unidades de tempo.

Imagine que queremos escolher entre 3 opções:

- opção 1: produzir 2 unidades de cada produto (_batch size_) por vez,

- opção 2: produzir 4 unidades de cada produto por vez,

- opção 3: produzir 8 unidades de cada produto por vez.

Em um intervalo de 20 unidades de tempo, as opções acima seriam algo como:

- opção 1: A A _ _ B B _ _ A A _ _ B B _ _ A A _ _ 

- opção 2: A A A A _ _ B B B B _ _ A A A A _ _ B B

- opção 3: A A A A A A A A _ _ B B B B B B B B _ _ 

Os resultados estão mostrados na tabela a seguir:

Opção  Qtde A    Qtde B   Total  Tempo de Setup
  1      6         4       10        10
  2      8         6       14         6
  3      8         8       16         4
  
  Numa primeira análise, vemos que há vantagem em produzir _batch sizes_ grandes, pois o resultado da produção é maior, e o tempo perdido com setup é menor.
  
  Infelizmente, este reaciocínio não é totalmente correto, porque os produtos gerados não foram totalmente *validados* apenas com o processo produtivo. É preciso esperar o produto chegar no mercado e termos o feedback do cliente. Considerando isso, os grandes _batch sizes_ representam um custo e não um benefício. 

### 2. Assess assumptions on which statistical inference will be based

```javascript
if (isAwesome){
  return true
}
```

### 3. Support the selection of appropriate statistical tools and techniques

<img src="images/dummy_thumbnail.jpg?raw=true"/>

### 4. Provide a basis for further data collection through surveys or experiments

Sed ut perspiciatis unde omnis iste natus error sit voluptatem accusantium doloremque laudantium, totam rem aperiam, eaque ipsa quae ab illo inventore veritatis et quasi architecto beatae vitae dicta sunt explicabo. 

For more details see [GitHub Flavored Markdown](https://guides.github.com/features/mastering-markdown/).
