# DataConnect: Análise de Indicadores Educacionais e Tecnológicos

<p align="center">
  <img src="edu08.jpg" alt="Logo Educação">
</p>

## Este é projeto final do curso de Análise de Dados | Turma On26 da [{Reprograma}](https://www.reprograma.com.br/).

## Introdução

No contexto contemporâneo, o acesso à internet desempenha um papel crucial no desenvolvimento das pessoas, proporcionando informações, entretenimento e, especialmente, oportunidades educacionais e de emprego. Para aqueles que residem em áreas remotas, a internet atua como um equalizador, garantindo oportunidades merecidas.

Uma educação de qualidade não apenas enriquece vidas, mas também cria oportunidades sociais essenciais para enfrentar os desafios globais. Ao longo dos séculos, o mundo evoluiu de uma época com acesso limitado à educação básica para uma em que a maioria possui, com melhorias notáveis nas taxas de alfabetização.

No entanto, a mera presença na escola não é suficiente; o conteúdo do aprendizado é crucial. Disparidades educacionais persistem, especialmente em países de baixa renda, onde muitas crianças não alcançam a alfabetização ao término do ensino fundamental, exacerbando as desigualdades globais de renda e a pobreza.

Este cenário é evidente em áreas como o interior do Brasil, onde as oportunidades para educação superior são limitadas. Apesar do desejo de frequentar uma universidade, muitos não têm condições de se mudar para centros urbanos maiores.

Graças ao acesso à internet, tornou-se possível realizar cursos de graduação à distância, permitindo a obtenção de diplomas de nível superior e melhorando significativamente as perspectivas de emprego para esses indivíduos. No âmbito deste projeto, focaremos na análise da educação global, destacando os desafios e oportunidades que moldam o futuro das gerações vindouras.
<br>
<br>

**[Apresentação do Projeto Final](https://www.canva.com/design/DAF2WO2gPtk/rNUsayiwSIDX4TaVPb3U8g/edit?utm_content=DAF2WO2gPtk&utm_campaign=designshare&utm_medium=link2&utm_source=sharebutton)**
<br>
<br>
## 📁 Arquitetura do Projeto

<br>

```
 📁DataConnect: Análise de Indicadores Educacionais e Tecnológicos
   |
   ||--📁 Final
   |    |- 📄 parte_I.ipynb
   |    |- 📄 educacao_na_rede.csv
   |
   ||--📁 datasets
   |  |
   |  |
   |  ||- 📄 Final.csv
   |  ||- 📄 gender-gap-education-levels.csv
   |  ||- 📄 learning-adjusted-years-of-school-lays.csv
   |  ||- 📄 World Population Datasets - Information is Beautiful - World Population 2023 by Country.csv
   ||
   ||
   ||
   ||
   |- 📄 readme.csv
   |- 📄 edu08.jpg
   |- 📄 Dashboard.png
   

```

<br>
<br>

# 👩🏾‍💻 Tecnologias e Dependências Utilizadas

<br>

| Ferramenta | Descrição |
| --- | --- |
| `Python` | Linguagem de programação. |
| `Pandas`    | Biblioteca criada para a linguagem Python para manipulação e análise de dados.|
| `Numpy`    | Biblioteca para a linguagem Python, que suporta o processamento de grandes, multi-dimensionais arranjos e matrizes. |
| `Matplotlib`   | Biblioteca de software para criação de gráficos e visualizações de dados em geral, feita para e da linguagem de programação Python.|
| `Seaborn`    | Ferramenta para plotagem dos mais variados tipos de gráficos em Python.|
| `Jupyter Notebook`| Aplicação web criada para desenvolver software de código aberto, padrões abertos e serviços para computação interativa em dezenas de linguagens de programação.|
| `Tableau`    | Plataforma de análise, exploração e gerenciamento de dados visuais.|
|`Googletran` | Biblioteca em Python que facilita a integração com a API de tradução do Google Translate, permitindo a tradução de texto entre idiomas de forma eficiente e a detecção automática de idiomas.|


<br>

## Perguntas de Pesquisa

Inspirado por experiências de pessoas conhecidas, o decidi investigar a relação entre o acesso à internet e o desenvolvimento educacional, guiado pelas seguintes perguntas de pesquisa:

1. **Como a taxa líquida de matrícula total no ensino fundamental varia ao longo dos anos?**
2. **Existe alguma correlação entre a assinatura de banda larga e o número de usuários de Internet?**
3. **Qual é a distribuição da assinatura de celular entre as diferentes localidades?**
4. **Como a razão bruta de matrícula combinada para educação superior varia entre gêneros?**
5. **Qual é a relação entre a assinatura de celular e a taxa líquida de matrícula combinada no ensino Médio?**

## Sobre o Projeto

Este repositório contém uma análise detalhada de indicadores educacionais e tecnológicos em diversas entidades ao redor do mundo. O projeto foi conduzido através da exploração de três DataFrames principais, fornecendo informações valiosas sobre indicadores educacionais e tecnológicos. Cada DataFrame possui colunas específicas que foram exploradas durante a análise.

### DataFrame [`df_conexao_internet`](https://www.kaggle.com/datasets/ashishraut64/internet-users/data)

A Internet é um sistema global de redes interconectadas de computadores que utiliza o conjunto de protocolos da Internet (TCP/IP) para a comunicação entre redes e dispositivos. Essa rede abrange desde redes locais até globais, públicas e privadas, acadêmicas, empresariais e governamentais. A interconexão ocorre por meio de diversas tecnologias, como redes eletrônicas, sem fio e ópticas. A Internet possibilita o transporte de uma ampla variedade de recursos e serviços, como documentos de hipertexto, aplicativos da World Wide Web (WWW), correio eletrônico, telefonia e compartilhamento de arquivos.

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

### DataFrame [`df_anos_de_escola`](https://www.kaggle.com/datasets/imtkaggleteam/global-education/data)

Anos de escola ajustados ao aprendizado: A discrepância na educação ao redor do mundo persiste, sendo medida pelo tempo que as crianças passam na escola. Pesquisadores também ajustam para a qualidade da educação usando "anos de escola ajustados ao aprendizado". O mapa revela grandes diferenças.

Em muitos países mais pobres, as crianças têm menos de três anos de educação de qualidade ajustada. Nos países ricos, esse número ultrapassa 10 anos. Nas áreas mais habitadas do Sul da Ásia e da África Subsaariana, onde a maioria das crianças reside, a média de anos de educação de qualidade é inferior a 7, indicando desafios persistentes na oferta de uma educação de alta qualidade nessas regiões.

#### Colunas:
- Entity: Entidade
- Code: Código
- Year: Ano
- Learning-Adjusted Years of School: Anos de Escola Ajustados para Aprendizado

#### Ações Realizadas:
- Verificação de valores nulos.
- Exibição dos primeiros e últimos valores.
- Descrição estatística das colunas.

### DataFrame [`df_educacao_genero`](https://www.kaggle.com/datasets/adamaboubacaroumarou/gender-gap-education)

Lacuna de gênero nos níveis de educação: Recentemente, esforços globais foram concentrados para superar a disparidade de gênero na educação. Antes, os meninos tinham mais chances de frequentar a escola do que as meninas, mas agora essa diferença desapareceu em grande parte.

Ao observar o gráfico das taxas de matrícula global no ensino fundamental, médio e superior, notamos que as linhas convergiram ao longo do tempo. Atualmente, as taxas de matrícula entre meninos e meninas são iguais, indicando um equilíbrio alcançado.

De maneira notável, no ensino superior, as mulheres jovens superam os homens jovens em termos de matrícula, representando uma mudança positiva no panorama educacional global.

#### Colunas:
- Entity: Entidade
- Code: Código
- Year: Ano
- Combined gross enrolment ratio for tertiary education, female: Taxa bruta de matrícula combinada para educação superior, feminina
- Combined gross enrolment ratio for tertiary education, male: Taxa bruta de matrícula combinada para educação superior, masculina
- Combined total net enrolment rate, secondary, male: Taxa de matrícula líquida total combinada, ensino médio, masculina
- Combined total net enrolment rate, secondary, female: Taxa de matrícula líquida total combinada, ensino médio, feminina
- Combined total net enrolment rate, primary, female: Taxa de matrícula líquida total combinada, ensino fundamental, feminina
- Combined total net enrolment rate, primary: Taxa de matrícula líquida total combinada, ensino fundamental

#### Ações Realizadas:
- Verificação de valores nulos.
- Exibição dos primeiros e últimos valores.
- Descrição estatística das colunas.

### DataFrame [`df_populacao_mundial`](https://www.un-ilibrary.org/content/books/9789210027137/read)

#### Colunas:
- Country, territory or other area: Localização
- Population (estimated mid-year value, millions): População (valor estimado, milhões)
- Region: Região

#### Ações Realizadas:
- Verificação de valores nulos.
- Exibição dos primeiros e últimos valores.
- Descrição estatística das colunas.

## Exploração Conjunta e Transformação

Após entender as informações em cada DataFrame, realizamos uma exploração conjunta. Unimos os três DataFrames em um novo DataFrame chamado `df_educacao_na_rede`. Renomeamos suas colunas para o português e exportamos os dados para um arquivo CSV chamado "educação_na_rede". Utilizamos a biblioteca Translator para traduzir os nomes dos países.

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

## [Dashboard](https://public.tableau.com/views/DataConnectAnlisedeIndicadoresEducacionaiseTecnolgicos/Painel1?:language=pt-BR&:display_count=n&:origin=viz_share_link)
