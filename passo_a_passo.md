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

