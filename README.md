É possível ler a url do banco de dados pelo link do "raw" no GitHub



`.sample()` retorna uma linha aleatória do DataFrame e tem como parâmetro a quantidade de linhas a serem retornadas



Para pegar somente a linha 6522 da coluna "Bairros", faz-se da seguinte forma:

```python
dados['Bairros'][6522]
```

separa-se primeiro o DataFrame em uma Series para então pegar somente o valor de tal linha



Para conseguir informações sobre tal conjunto de dados, usa-se o `.info()`



É possível montar gráficos somente com a biblioteca do Pandas da seguinte forma:

```python
qtd_bairros = dados['Bairros'].value_counts()

qtd_bairros.head(10).plot.bar()

>>>
```

![image-20220527223053435](C:\Users\Marco Neto\AppData\Roaming\Typora\typora-user-images\image-20220527223053435.png)

foi pego somente os 10 primeiros itens senão o gráfico ficaria desorganizado com tanto dado em tão pouca tela



um Jupyter Notebook é um Storytelling, por possuir blocos de código e de texto, podendo até ser adicionado imagens