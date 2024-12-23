### Teste de Analista de Dados

Depois de criar o Fork do projeto, fazer o download da base e do dicionário, analizar e entender a base disponibilizada:
- Criação do diagrama de dados
    - Para evitar a duplicação de dados, mas mantendo a separação por categoria, procurei separar as tabelas de modo que haja uma redução no espaço em disco utilizado. 
    - O tipo dos dados foi definido com o objetivo de reduzir o espaço em disco utilizado e otimizar a performance dos cálculos.
    - O diagrama está disponível no repositório ('Diagrama.pdf')
- Criação do container no Docker
- Configuração do MySQL no container

As próximas etapas seguidas são encontradas nos blocos de código abaixo, seguindo a ordem cronológica adotada.
- Criação do jupyter notebook
- Instalação e importação das bibliotecas
- Conexão com o BD via SQLAlchemy
- Leitura do arquivo csv e alteração dos tipos de dados do Dataframe
- Criação das tabelas, tipagem de dados e importação no BD
- Criação, carregamento e importação das Tabelas Dicionário no BD
- Criação do arquivo de indicadores levantados em Excel. Aqui vimos a necessidade de ajustar o banco, por isso, o diagrama foi ajustado para atender as necessidades do teste.
    - O arquivo está disponível [clicando aqui](https://docs.google.com/spreadsheets/d/1de-xZhzdkAc_e99nKchbXzaJc1hEG4fH/edit?usp=sharing&ouid=103709149943287631455&rtpof=true&sd=true)
- Criação do arquivo de visões em Excel.
    - O arquivo está disponível [clicando aqui](https://docs.google.com/spreadsheets/d/1-msRg5k1M1YlXqOCOGfH4E_ZLjU3hK5e/edit?usp=sharing&ouid=103709149943287631455&rtpof=true&sd=true)

Bullets:
1.	Analisando o Mapa Coroplético, percebemos que as regiões mais desenvolvidas (Sul e Sudeste) e com maior acesso a educação são as que possuem as maiores médias de notas. Essa desigualdade está ainda mais presente quando filtramos apenas escolas públicas.
2.	O Gráfico de radar mostra a desigualdade social étnica presente no Brasil, principalmente com a população indígena.
3.	Na tabela presente no Painel de Notas, é possível verificar que os inscritos que não possuem presença em todas as provas estão sujeitos a ter uma média menor, mesmo considerando apenas as notas das provas realizadas. Isso pode acontecer pois uma performance aquém pode levar a desistência do segundo dia de provas, ou a uma desmotivação no caso de uma falta no primeiro dia.
4.	 No Painel Redação e Socioeconômico podemos utilizar os filtros para perceber detalhes na relação entre a nota das provas e a nota da redação. A população preta teve uma dificuldade maior na nota das provas em relação a redação, e a população indígena teve uma dificuldade maior na nota da redação em relação as provas.
5.	Utilizando o filtro de Sexo no Painel Redação e Socioeconômico, percebemos que as pessoas do sexo feminino possuem uma maior facilidade na escrita para a redação, e as pessoas do sexo masculino possuem uma maior facilidade nas questões da prova.
6.	Entre os inscritos que zeraram a redação, mais de um terço a deixou em branco.
7.	 No painel socioeconômico, percebemos que o fato de ter internet em casa é um fator que impacta diretamente no desempenho do inscrito, visto que a média das notas aumenta em 57 pontos para os que a possuem.
8.	O gráfico de Média por Escolaridade dos Pais mostra o impacto da educação que os pais receberam na educação dos filhos, sendo proporcional a nota das provas.
9.	Assim como era esperado, a renda familiar também está diretamente ligada à média dos inscritos, como podemos ver no gráfico de Média por Renda.
10.	Em todos os gráficos de todos os painéis, podemos ver o impacto do tipo de escola (pública ou privada) na nota dos alunos. Em todas as visualizações, as notas das escolas privadas são maiores.
