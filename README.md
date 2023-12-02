# DataConnect: Análise de Indicadores Educacionais e Tecnológicos

## Introdução

No contexto atual, o acesso à internet tornou-se crucial para o desenvolvimento das pessoas, proporcionando acesso a informações, educação, entretenimento e oportunidades de emprego.

Para aqueles que residem em áreas remotas, o acesso à internet desempenha um papel especialmente importante, uma vez que essas pessoas podem não ter as mesmas oportunidades educacionais e de emprego que aquelas que vivem em centros urbanos. A internet atua como um equalizador, oferecendo oportunidades merecidas a essas pessoas.

como o caso de indivíduos que nasceram e cresceram em cidades do interior do Brasil, onde as oportunidades de educação superior eram limitadas. Apesar do desejo de frequentar uma universidade, muitos não tinham condições de se mudar para uma cidade maior.

Graças ao acesso à internet, foi possível realizar cursos de graduação à distância, possibilitando a obtenção de diplomas de nível superior e a melhoria das perspectivas de emprego.

## Perguntas de Pesquisa

Inspirado por experiências de pessoas conhecidas, o decidi investigar a relação entre o acesso à internet e o desenvolvimento educacional, guiado pelas seguintes perguntas de pesquisa:

1. **Como a taxa líquida de matrícula total no ensino primário varia ao longo dos anos?**
2. **Existe alguma correlação entre a assinatura de banda larga e o número de usuários de Internet?**
3. **Qual é a distribuição da assinatura de celular entre as diferentes localidades?**
4. **Como a razão bruta de matrícula combinada para educação terciária varia entre gêneros?**
5. **Qual é a relação entre a assinatura de celular e a taxa líquida de matrícula combinada no ensino secundário?**

## Sobre o Projeto

Este repositório contém uma análise detalhada de indicadores educacionais e tecnológicos em diversas entidades ao redor do mundo. O projeto foi conduzido através da exploração de três DataFrames principais, fornecendo informações valiosas sobre indicadores educacionais e tecnológicos. Cada DataFrame possui colunas específicas que foram exploradas durante a análise.

### DataFrame [`df_conexao_internet`](https://www.kaggle.com/datasets/ashishraut64/internet-users/data)

#### Colunas:
- Entity: Entidade
- Code: Código
- Year: Ano
- Cellular Subscription: Assinatura de Celular
- Internet Users(%): Usuários de Internet (%)
- No. of Internet Users: Número de Usuários de Internet
- Broadband Subscription: Assinatura de Banda Larga

#### Ações Realizadas:
- Verificação de valores nulos.
- Exibição dos primeiros e últimos valores.
- Descrição estatística das colunas.

### DataFrame [`df_anos_de_escola`](https://www.kaggle.com)

#### Colunas:
- Entity: Entidade
- Code: Código
- Year: Ano
- Learning-Adjusted Years of School: Anos de Escola Ajustados para Aprendizado

#### Ações Realizadas:
- Verificação de valores nulos.
- Exibição dos primeiros e últimos valores.
- Descrição estatística das colunas.

### DataFrame [`df_educacao_genero`](https://www.kaggle.com)

#### Colunas:
- Entity: Entidade
- Code: Código
- Year: Ano
- Combined gross enrolment ratio for tertiary education, female: Taxa bruta de matrícula combinada para educação superior, feminina
- Combined gross enrolment ratio for tertiary education, male: Taxa bruta de matrícula combinada para educação superior, masculina
- ...

#### Ações Realizadas:
- Verificação de valores nulos.
- Exibição dos primeiros e últimos valores.
- Descrição estatística das colunas.

## Exploração Conjunta e Transformação

Após entender as informações em cada DataFrame, realizamos uma exploração conjunta. Unimos os três DataFrames em um novo DataFrame chamado `df_educacao_na_rede`. Renomeamos suas colunas para o português e exportamos os dados para um arquivo CSV chamado "educação_na_rede". Utilizamos a biblioteca Translator para traduzir os nomes dos países.

## Visualizações em Gráficos

Abaixo estão algumas das perguntas respondidas por meio de gráficos usando a biblioteca matplotlib:


# Importar as bibliotecas necessárias
from googletrans import Translator
import pandas as pd
import matplotlib.pyplot as plt
import seaborn as sns

# Carregar DataFrames
df_conexao_internet = pd.read_csv('caminho/do/arquivo/df_conexao_internet.csv')
df_anos_de_escola = pd.read_csv('caminho/do/arquivo/df_anos_de_escola.csv')
df_educacao_genero = pd.read_csv('caminho/do/arquivo/df_educacao_genero.csv')
df_educacao_na_rede = pd.read_csv('caminho/do/arquivo/educacao_na_rede.csv')

## Análise Exploratória

A análise exploratória dos dados revelou insights importantes:

- A taxa líquida de matrícula total no ensino primário tem apresentado crescimento nos últimos anos.
- Existe uma correlação positiva entre assinatura de banda larga e o número de usuários de Internet.
- A assinatura de celular é mais prevalente em localidades mais populosas.
- A razão bruta de matrícula para educação terciária é mais elevada para homens do que para mulheres.
- Há uma correlação positiva entre a assinatura de celular e a taxa líquida de matrícula combinada no ensino secundário.

## Conclusão

Com base na análise dos dados, destacam-se os seguintes pontos:

1. **Crescimento de Usuários de Internet e Assinaturas de Banda Larga:**
   - Observa-se um crescimento tanto no número de usuários de internet quanto nas assinaturas de banda larga. Os usuários aumentam mais rapidamente do que as assinaturas de banda larga, indicando uma maior penetração da internet em diversas regiões. Países como Sudão do Sul apresentam menor quantidade de assinaturas de internet no celular, enquanto Macau lidera em assinaturas de internet no celular.

2. **Educação e Matrículas:**
   - No âmbito educacional, nota-se que o sexo masculino possui um número maior de matrículas, embora tenha havido uma queda em 2017 para ambos os gêneros, especialmente no ensino primário em escala global. Os anos ajustados de aprendizado e as assinaturas de banda larga nos países mostram uma tendência de crescimento conjunto.

3. **Taxa de Matrícula e Assinaturas de Celular:**
   - A relação entre a taxa de matrícula secundária do gênero masculino e as assinaturas de celular no mundo não apresenta uma tendência clara. Entretanto, a taxa de matrícula feminina no ensino primário cresceu significativamente em 2018.

4. **Desafios na Adoção de Banda Larga:**
   - Ainda há pessoas sem assinatura de banda larga, embora o número seja baixo e sem uma tendência clara. A relação entre anos de escola e assinaturas de banda larga está em crescimento.

5. **Acesso à Internet na América do Sul:**
   - Na América do Sul, o Brasil é destacado como o país com maior acesso à internet. Em 2018, o Peru lidera em número de casas com acesso à internet.

Os resultados indicam que o acesso à internet desempenha um papel fundamental no desenvolvimento educacional, proporcionando oportunidades de aprendizado global e contribuindo para a melhoria da qualidade da educação.

## Recomendações

Com base nos resultados da análise, são feitas as seguintes recomendações:

- Investir em políticas públicas que promovam o acesso à internet, especialmente para famílias de baixa renda e localidades com menor população.
- Apoiar o desenvolvimento de cursos online de qualidade, especialmente em áreas como tecnologia e educação.
