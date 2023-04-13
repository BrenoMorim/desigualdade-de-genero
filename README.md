# Analisando a desigualdade de gênero no Brasil

> Status: Concluído

Análise com base na PNAD de 2015, com o conteúdo aprendido nos cursos de estatística com python da Alura. O objetivo do projeto é mostrar a desigualdade no Brasil.

| :placard: Vitrine.Dev |     |
| -------------  | --- |
| :sparkles: Nome        | **Desigualdade de Gênero no Brasil**
| :label: Tecnologias | Python, Jupyter Notebook

![Gráfico mostrando a distribuição de renda entre as mulheres chefes de família](https://github.com/BrenoMorim/desigualdade-de-genero/blob/main/imagem-do-projeto.png?raw=true#vitrinedev)

## Detalhes do Projeto

Foram utilizados dados da Pesquisa Nacional de Amostra a Domícilio de 2015 do IBGE para demonstrar a desigualdade de gênero no Brasil. Os treinamentos de estatística com Python da Alura serviram como base no desenvolvimento, assim como os dados da PNAD já tratados. Foram analisados como a distribuição de renda e nível de estudo variam dependendo do gênero, fazendo testes estatísticos, regressões e análises gráficas com boxplots e histogramas.O objetivo dessa análise foi simplesmente demonstrar de forma estatística que a desigualdade existe, sem discutir o porquê dela existir ou como solucionar esse problema.

## Alguns gráficos e análises

### Proporção entre homens e mulheres chefes de família

De acordo com a PNAD de 2015, aproximadamente 69,3% das famílias têm um homem como provedor principal, enquanto 30,7% têm uma mulher como provedora. O que é muito discrepante da proporção populacional entre homens e mulheres, além de que a maioria das famílias com uma mulher como chefe, são assim por conta da ausência da figura paterna.

## Analisando a renda

### Renda dos homens

![Histograma mostrando a renda dos homens chefes de família](./graficos/renda_homens.png)

### Renda das mulheres

![Histograma mostrando a renda das mulheres chefes de família](./graficos/renda_mulheres.png)

Podemos ver que em ambos os casos, a maioria das pessoas recebe apenas um salário mínimo, que na época era 788 reais. Porém, podemos perceber que existe uma quantidade bem maior de homens que ganham salários maiores, como 2000, 4000, 5000, 6000 e 10000 do que mulheres. Além disso, há mais mulheres que ganham salários menores do que um salário mínimo em comparação com os homens.

## Analisando o estudo

### Estudo dos homens

![Histograma mostrando o estudo dos homens chefes de família](./graficos/estudo_homens.png)

### Estudo das mulheres

![Histograma mostrando o estudo das mulheres chefes de família](./graficos/estudo_mulheres.png)

Podemos ver que há uma maior concetração em 11 anos de estudo, que corresponde à conclusão do ensino médio. Nesses gráficos podemos perceber uma contradição com os gráficos anteriores sobre renda, porque há uma maior quantidade de homens que não concluíram o ensino médio e até que não tem nenhum estudo se compararmos com as mulheres. Notamos que as mulheres chefes de família geralmente possuem mais estudo, quase 20% possuem ensino superior e mais de 30% finalizaram somente o ensino médio, ao contrário dos homens, pouco mais de 10% dos homens chefes de família possuem ensino superior.

#### Podemos então chegar à conclusão de que mesmo estudando mais, as mulheres acabam tendo uma renda menor no geral.

### Renda por etnia e gênero

![Box plot mostrando a renda dos chefes de família por etnia e gênero](./graficos/boxplot_renda.png)

É notável que em todas as etnias, o gênero masculino acaba prevalecendo sobre o feminino nessa questão, sendo que a etnia amarela é aquela que possui a maior renda, seguida da etnia branca, parda, preta e indígena.

### Estudo por etnia e gênero

![Box plot mostrando os anos de estudo dos chefes de família por etnia e gênero](./graficos/boxplot_estudo.png)

Já nesse gráfico representando os anos de estudo, podemos notar que no geral, as mulheres chefes de família possuem mais estudo que os homens na mesma posição. As etnias com mais estudo seguem o mesmo padrão da renda, sendo a etnia amarela com mais estudo, seguida pela branca, parda, preta e indígena.

### Usando regressão

Por fim, é possível usar regressão para representar a distribuição de renda no Brasil com fórmulas, claro que de forma pouco precisa, com o objetivo de somente constatar a desigualdade, visto que a renda é influenciada por muitos outros fatores. Usando somente os dados da PNAD 2015, considerando somente o estado de SP e pessoas com renda entre 300 e 10000, obtemos as seguintes fórmulas:

- **Geral: Renda = 534,06 + 166,97 * Anos de Estudo**
- **Homens: Renda = 668,53 + 175,21 * Anos de Estudo**
- **Mulheres: Renda = 78,30 + 165,54 * Anos de Estudo**

Com base nesses dados, uma mulher com ensino superior completo ganharia R$2.561,42, enquanto um homem na mesma posição teria uma renda de R$3.296,70, sendo uma diferença de R$735,28. Lembrando que esses dados não conseguem prever com precisão a renda de ninguém (ainda mais considerando que foram usados dados de 2015, e desde então houveram mudanças no valor do real e no poder de compra) e que estão sendo usados simplesmente para ilustrar a desigualdade de forma estatística.

---
