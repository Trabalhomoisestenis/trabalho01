# TRABALHO 01:  Título do Trabalho
Trabalho desenvolvido durante a disciplina de Banco de Dados do Integrado

# Sumário

### 1. COMPONENTES<br>
Integrantes do grupo<br>
Davi Moura:mouradavi12@gmail.com
Calebe Carias:calebecarias@gmail.com
...

### 2.INTRODUÇÃO E MOTIVAÇAO<br>
Este documento contém a especificação do projeto do banco de dados <nome do projeto> 
<br>e motivação da escolha realizada. <br>

> A empresa “tenON” visa criar projetos para colaborar para a melhora da saúde da sociedade.
Para ajudar as pessoas a melhorar seus desempenhos na prática de atividade física, quisemos
desenvolver esse projeto. Os tênis da linha “shoesqdele”, que contem um sensor cujo objetivo é gerenciar todas as
informações ao desenvolvimento das atividades físicas do usuário. Para fazer isso o sistema
tem que armazenar informações relativas as atividades físicas praticadas, como: Distância
percorrida, peso, calorias gastas e velocidade média. O sistema deverá gerar relatórios que
ajudarão o usuário com sua performance.
 

### 3.MINI-MUNDO Novo<br>

Descrever o mini-mundo! (Não deve ser maior do que 30 linhas) <br>
Entrevista com o usuário e identificação dos requisitos.<br>
Descrição textual das regras de negócio definidas como um  subconjunto do mundo real 
cujos elementos são propriedades que desejamos incluir, processar, armazenar, 
gerenciar, atualizar, e que descrevem a proposta/solução a ser desenvolvida.

> O sistema proposto para os tênis "shoesqdele" conterá as informações aqui detalhadas. Serão
armazenados do usuario: nome,data de nascimento,sexo,altura inicial de seu progresso, rg, peso inicial. Ao longo do tempo o usuário será capaz de atualizar os valores de seu peso e sua altura  e as respectivas datas da mudança.Serão armazenados pelo sensor: seu código, as coordenadas do percurso do usuário ao longo da prática de seu exercicio e tempo de exercício feito. Dos tenis serao guardados os seguintes dados:o nome do modelo e o seu código, além de sua especialidade. Do tipo de exercicio serão armazenados: O nome do exercício e a quantidade media de calorias gastas por hora.

## Marco de Entrega 01 em: (06/05/2019)<br>

### 4.RASCUNHOS BÁSICOS DA INTERFACE (MOCKUPS)<br>
Neste ponto a codificação não e necessária, somente as ideias de telas devem ser desenvolvidas. O princípio aqui é pensar na criação da interface para identificar possíveis informações a serem armazenadas e/ou descartadas <br>

Sugestão: https://balsamiq.com/products/mockups/<br>

![Alt text](https://github.com/Trabalhomoisestenis/trabalho01/blob/master/balsamiq.png)
![Arquivo PDF do Protótipo Balsamiq feito para empresa tenON](https://github.com/Trabalhomoisestenis/trabalho01/blob/master/New%20Project%20copy%202.pdf)

## Marco de Entrega 02 em: (08/05/2019)<br>

#### 4.1 QUAIS PERGUNTAS PODEM SER RESPONDIDAS COM O SISTEMA PROPOSTO?
    a) O sistema proposto poderá fornecer quais tipos de relatórios e informaçes? 
    b) Crie uma lista com os 5 principais relatórios que poderão ser obtidos por meio do sistema proposto!
    
> A Empresa tenON precisa inicialmente dos seguintes relatórios:
*Relatório que informe o desempenho do usuário após a atividade física incluindo as calorias gastas, distância percorrida e o tempo gasto.
Relatório que informe os tênis mais usados pelos usuários para fazer os exercícios
Relatorio que informe os  exercicios mais realizados pelos usuarios
Relatorio que informe a media de calorias gastas de um usuario
*Relatório que informe o progresso do peso do usuário de acordo com sua meta mensal

## Marco de Entrega 03 em: (13/05/2019)<br>

#### 4.2 TABELA DE DADOS DO SISTEMA:
    a) Esta tabela deve conter todos os atributos do sistema e um mínimo de 10 linhas/registros de dados.
    b) Esta tabela tem a intenção de simular um relatório com todos os dados que serão armazenados 
    e deve ser criada antes do modelo conceitual
    c) Após criada esta tabela não deve ser modificada, pois será comparada com os resultados finais na conclusão do trabalho
    
    
    
    
    
    
    (    https://github.com/Trabalhomoisestenis/trabalho01/blob/master/shoestabela.ods)

## Marco de Entrega 04 em: (15/05/2019)<br>

### 5.MODELO CONCEITUAL<br>
    A) NOTACAO ENTIDADE RELACIONAMENTO 
        * Para nosso prótótipo limitaremos o modelo conceitual nas 5 principais entidades do escopo
        * O protótipo deve possui no mínimo duas relações N para N
        * o mínimo de entidades do modelo conceitual será igual a 5
        
![Alt text](https://github.com/Trabalhomoisestenis/trabalho01/blob/master/picmodeconc.png)
    B) QUALIDADE 
        Garantir que a semântica dos atributos seja clara no esquema
        Criar o esquema de forma a garantir a redução de informação redundante, possibilidade de valores null, 
        e tuplas falsas
    
        
    
#### 5.1 Validação do Modelo Conceitual
    [Grupo01]: [Nomes dos que participaram na avaliação]
    [Grupo02]: [Nomes dos que participaram na avaliação]
    
## Marco de Entrega 05 em: (20/05/2019)<br>

#### 5.2 DESCRIÇÃO DOS DADOS 
   USUÁRIO: Tabela que armazena as informações relativas ao usuário.

	RG: Campo que armazena o número do Registro Geral de cada usuário.
	
	Nome: Campo que armazena o nome do usuário.

	Idade: Campo que armazena a idade do usuário.
	
	Peso Inicial: Campo que armazena o peso inicial do usuário ao entrar no aplicativo.

	Sexo: Campo que armazena o sexo do usuário.
	
	Altura: Campo que armazena a altura do usuário



TÊNIS: Tabela que armazena as informações relativas ao tênis adquirido pelo usuário.	
	
	Código_Tênis: Campo que armazena o código específico de um tênis.

	Modelo: Campo que armazena o modelo do tênis.

	Especialidade: Campo que armazena a especialidade do exercício do tênis.



SENSOR: Tabela que armazena as informações relativas ao sensor adquirido pelo usuário:

	Código_Sensor: Campo que armazena o código do sensor.
	
	

Tipo de Exercícios: Tabela que armazena as informações relativas a cada exercício:

	Nome: Campo que armazena o nome do exercício

	Calorias_gastas_hora: Campo que armazena a quantidade de calorias gastas por hora 
	que aquele exercício específico promove 
	
	Código: Campo que armazena o código do exercício
    
  
## Marco de Entrega 06 em: (22/05/2019)<br>

### 6	MODELO LÓGICO<br>
![Alt text](https://github.com/Trabalhomoisestenis/trabalho01/blob/master/picmodelog.png)
### 7	MODELO FÍSICO<br>
       
       j

CREATE TABLE Usuario (
    RG int PRIMARY KEY,
    Nome varchar(100),
    Idade int,
    Peso_Inicial float,
    Sexo char(1),
    Altura float
);

CREATE TABLE Tenis (
    Codigo_Tenis int PRIMARY KEY,
    Modelo varchar(40),
    Especialidade varchar(100)
);

CREATE TABLE Sensor (
    Codigo_Sensor int PRIMARY KEY
);

CREATE TABLE tipo_de_exercicio (
    Nome varchar(40),
    calorias_horas float,
    Codigo int PRIMARY KEY
);

CREATE TABLE Exercicio (
    data_inicio date,
    data_fim date,
    Latitude float,
    Longitude float,
    Horario_Inicio time,
    Horario_Fim time,
    Calorias_Gastas float,
    Peso_atual float,
    fk_tipo_de_exercicio_Codigo int,
    fk_Usuario_RG int,
    fk_Sensor_Codigo_Sensor int,
    fk_Tenis_Codigo_Tenis int
);
 
ALTER TABLE Exercicio ADD CONSTRAINT FK_Exercicio_1
    FOREIGN KEY (fk_tipo_de_exercicio_Codigo)
    REFERENCES tipo_de_exercicio (Codigo)
    ON DELETE RESTRICT;
 
ALTER TABLE Exercicio ADD CONSTRAINT FK_Exercicio_2
    FOREIGN KEY (fk_Usuario_RG)
    REFERENCES Usuario (RG)
    ON DELETE RESTRICT;
 
ALTER TABLE Exercicio ADD CONSTRAINT FK_Exercicio_3
    FOREIGN KEY (fk_Sensor_Codigo_Sensor)
    REFERENCES Sensor (Codigo_Sensor)
    ON DELETE RESTRICT;
 
ALTER TABLE Exercicio ADD CONSTRAINT FK_Exercicio_4
    FOREIGN KEY (fk_Tenis_Codigo_Tenis)
    REFERENCES Tenis (Codigo_Tenis)
    ON DELETE RESTRICT;
## Marco de Entrega 07 em: (27/05/2019)<br>

### 8	INSERT APLICADO NAS TABELAS DO BANCO DE DADOS<br>
#### 8.1 DETALHAMENTO DAS INFORMAÇÕES

INSERT INTO SENSOR(codigo_sensor) VALUES(4321),(5432),(6543),(7654),(8765),(9876),(1987),(2987),(3987),(4874);


INSERT INTO tipo_de_exercicio (codigo,nome,calorias_horas) VALUES (1,'futebol',760),(2,'basquete',584),(3,'corrida_obstaculo',715),(4,'golfe',315),(5,'volei',350),(6,'tenis',610),(7,'corrida',610),(8,'futebol americano',580),(9,'remo',470),(10,'caminhada',440); 

INSERT INTO USUARIO (rg,nome,idade,peso_inicial,sexo,altura) VALUES (12345,'Calebe',17,59,'M',1.71),(23456,'Davi',15,60,'M',1.75),(34567,'Alessandra',25,65,'F',1.82),(45678,'Rodolfo',22,71,'M',1.71),(56789,'Gustavo',33,82,'M',1.82),(67890,'Buteri',13,47,'M',1.73),(11234,'Maira',18,58,'F',1.91),(22345,'Rosilene',31,67,'F',1.55),(33456,'Felipe Noronha',27,62,'M',1.7),(44567,'Pedro',60,35,'M',1.61)


INSERT INTO TENIS (Codigo_tenis, Modelo, especialidade) VALUES (1010, 'Nike1v9', 'futebol'), (2020, 'Penalty', 'basquete'),(3030, 'Adidas3', 'volei'),(4040, 'Hypervenom', 'corrida'),(5050, 'Umbro', 'Golfe'),(6060, 'Puma', 'Corrida'),(7070, 'Umbro2', 'futebol'),(8080, 'Havaianas', 'futsal'),(9090, 'Nike', 'corrida'),(1212, 'Adidas2', 'Basquete');


INSERT INTO EXERCICIO(data_inicio,data_fim,latitude,longitude,horario_inicio,horario_fim,calorias_gastas,peso_atual,fk_tipo_de_exercicio_codigo,fk_usuario_rg,fk_sensor_codigo_sensor,fk_tenis_codigo_tenis) VALUES('2019-06-30','2019-06-30',-23.6506557,-46.5603576,'16:00','17:00',760,59,1,12345,4321,1010),('2019-07-01','2019-07-01',-19.9215223,-43.9340913,'17:00','18:00',584,60,2,23456,5432,2020),('2019-07-02','2019-07-02',34.0326511,-118.4602074,'18:00','19:00',715,65,3,34567,6543,3030),('2019-07-03','2019-07-03',33.8993738,-118.3787682,'19:00','20:00',315,71,4,45678,7654,4040),('2019-07-04','2019-07-04',37.4030185,-122.3212805,'20:00','21:00',350,82,5,56789,8765,5050),('2019-07-05','2019-07-05',24.3781314,-80.4603501,'21:00','22:00',610,47,6,67890,9876,6060),('2019-07-06','2019-07-06',22.3531176,113.8475127,'22:00','23:00',610,58,7,11234,1987,7070),('2019-07-07','2019-07-07',25.0000188,-71.0087548,'23:00','00:00',580,67,8,22345,2987,8080),('2019-07-08','2019-07-09',-25.7663566,-49.7417204,'00:00','01:00',470,62,9,33456,3987,9090),('2019-07-09','2019-07-09',43.7184038,-79.5181409,'01:00','02:00',440,35,10,44567,4874,1212);



#### 8.2 INCLUSÃO DO SCRIPT PARA CRIAÇÃO DE TABELA E INSERÇÃO DOS DADOS 


CREATE TABLE Usuario ( RG int PRIMARY KEY, Nome varchar(100), Idade int, Peso_Inicial float, Sexo char(1), Altura float );

CREATE TABLE Tenis ( Codigo_Tenis int PRIMARY KEY, Modelo varchar(40), Especialidade varchar(100) );

CREATE TABLE Sensor ( Codigo_Sensor int PRIMARY KEY );

CREATE TABLE tipo_de_exercicio ( Nome varchar(40), calorias_horas float, Codigo int PRIMARY KEY );

CREATE TABLE Exercicio ( data_inicio date, data_fim date, Latitude float, Longitude float, Horario_Inicio time, Horario_Fim time, Calorias_Gastas float, Peso_atual float, fk_tipo_de_exercicio_Codigo int, fk_Usuario_RG int, fk_Sensor_Codigo_Sensor int, fk_Tenis_Codigo_Tenis int );

ALTER TABLE Exercicio ADD CONSTRAINT FK_Exercicio_1 FOREIGN KEY (fk_tipo_de_exercicio_Codigo) REFERENCES tipo_de_exercicio (Codigo) ON DELETE RESTRICT;

ALTER TABLE Exercicio ADD CONSTRAINT FK_Exercicio_2 FOREIGN KEY (fk_Usuario_RG) REFERENCES Usuario (RG) ON DELETE RESTRICT;

ALTER TABLE Exercicio ADD CONSTRAINT FK_Exercicio_3 FOREIGN KEY (fk_Sensor_Codigo_Sensor) REFERENCES Sensor (Codigo_Sensor) ON DELETE RESTRICT;

ALTER TABLE Exercicio ADD CONSTRAINT FK_Exercicio_4 FOREIGN KEY (fk_Tenis_Codigo_Tenis) REFERENCES Tenis (Codigo_Tenis) ON DELETE RESTRICT;

INSERT INTO SENSOR(codigo_sensor) VALUES(4321),(5432),(6543),(7654),(8765),(9876),(1987),(2987),(3987),(4874);

INSERT INTO tipo_de_exercicio (codigo,nome,calorias_horas) VALUES (1,'futebol',760),(2,'basquete',584),(3,'corrida_obstaculo',715),(4,'golfe',315),(5,'volei',350),(6,'tenis',610),(7,'corrida',610),(8,'futebol americano',580),(9,'remo',470),(10,'caminhada',440);

INSERT INTO USUARIO (rg,nome,idade,peso_inicial,sexo,altura) VALUES (12345,'Calebe',17,59,'M',1.71),(23456,'Davi',15,60,'M',1.75),(34567,'Alessandra',25,65,'F',1.82),(45678,'Rodolfo',22,71,'M',1.71),(56789,'Gustavo',33,82,'M',1.82),(67890,'Buteri',13,47,'M',1.73),(11234,'Maira',18,58,'F',1.91),(22345,'Rosilene',31,67,'F',1.55),(33456,'Felipe Noronha',27,62,'M',1.7),(44567,'Pedro',60,35,'M',1.61);

INSERT INTO TENIS (Codigo_tenis, Modelo, especialidade) VALUES (1010, 'Nike1v9', 'futebol'), (2020, 'Penalty', 'basquete'),(3030, 'Adidas3', 'volei'),(4040, 'Hypervenom', 'corrida'),(5050, 'Umbro', 'Golfe'),(6060, 'Puma', 'Corrida'),(7070, 'Umbro2', 'futebol'),(8080, 'Havaianas', 'futsal'),(9090, 'Nike', 'corrida'),(1212, 'Adidas2', 'Basquete');

INSERT INTO EXERCICIO(data_inicio,data_fim,latitude,longitude,horario_inicio,horario_fim,calorias_gastas,peso_atual,fk_tipo_de_exercicio_codigo,fk_usuario_rg,fk_sensor_codigo_sensor,fk_tenis_codigo_tenis) VALUES('2019-06-30','2019-06-30',-23.6506557,-46.5603576,'16:00','17:00',760,59,1,12345,4321,1010),('2019-07-01','2019-07-01',-19.9215223,-43.9340913,'17:00','18:00',584,60,2,23456,5432,2020),('2019-07-02','2019-07-02',34.0326511,-118.4602074,'18:00','19:00',715,65,3,34567,6543,3030),('2019-07-03','2019-07-03',33.8993738,-118.3787682,'19:00','20:00',315,71,4,45678,7654,4040),('2019-07-04','2019-07-04',37.4030185,-122.3212805,'20:00','21:00',350,82,5,56789,8765,5050),('2019-07-05','2019-07-05',24.3781314,-80.4603501,'21:00','22:00',610,47,6,67890,9876,6060),('2019-07-06','2019-07-06',22.3531176,113.8475127,'22:00','23:00',610,58,7,11234,1987,7070),('2019-07-07','2019-07-07',25.0000188,-71.0087548,'23:00','00:00',580,67,8,22345,2987,8080),('2019-07-08','2019-07-09',-25.7663566,-49.7417204,'00:00','01:00',470,62,9,33456,3987,9090),('2019-07-09','2019-07-09',43.7184038,-79.5181409,'01:00','02:00',440,35,10,44567,4874,1212);
 
#### 8.3 INCLUSÃO DO SCRIPT PARA EXCLUSÃO DE TABELAS EXISTENTES, CRIAÇÃO DE TABELA NOVAS E INSERÇÃO DOS DADOS
   DROP TABLE exercicio;
   DROP TABLE usuario;
   DROP TABLE TENIS;
  DROP TABLE tipo_de_exercicio;
  DROP TABLE sensor;
CREATE TABLE Usuario (
    RG int PRIMARY KEY,
    Nome varchar(100),
    Idade int,
    Peso_Inicial float,
    Sexo char(1),
    Altura float
);

CREATE TABLE Tenis (
    Codigo_Tenis int PRIMARY KEY,
    Modelo varchar(40),
    Especialidade varchar(100)
);

CREATE TABLE Sensor (
    Codigo_Sensor int PRIMARY KEY
);

CREATE TABLE tipo_de_exercicio (
    Nome varchar(40),
    calorias_horas float,
    Codigo int PRIMARY KEY
);

CREATE TABLE Exercicio (
    data_inicio date,
    data_fim date,
    Latitude float,
    Longitude float,
    Horario_Inicio time,
    Horario_Fim time,
    Calorias_Gastas float,
    Peso_atual float,
    fk_tipo_de_exercicio_Codigo int,
    fk_Usuario_RG int,
    fk_Sensor_Codigo_Sensor int,
    fk_Tenis_Codigo_Tenis int
);
 
ALTER TABLE Exercicio ADD CONSTRAINT FK_Exercicio_1
    FOREIGN KEY (fk_tipo_de_exercicio_Codigo)
    REFERENCES tipo_de_exercicio (Codigo)
    ON DELETE RESTRICT;
 
ALTER TABLE Exercicio ADD CONSTRAINT FK_Exercicio_2
    FOREIGN KEY (fk_Usuario_RG)
    REFERENCES Usuario (RG)
    ON DELETE RESTRICT;
 
ALTER TABLE Exercicio ADD CONSTRAINT FK_Exercicio_3
    FOREIGN KEY (fk_Sensor_Codigo_Sensor)
    REFERENCES Sensor (Codigo_Sensor)
    ON DELETE RESTRICT;
 
ALTER TABLE Exercicio ADD CONSTRAINT FK_Exercicio_4
    FOREIGN KEY (fk_Tenis_Codigo_Tenis)
    REFERENCES Tenis (Codigo_Tenis)
    ON DELETE RESTRICT;
    
    
    
    
INSERT INTO SENSOR(codigo_sensor) VALUES(4321),(5432),(6543),(7654),(8765),(9876),(1987),(2987),(3987),(4874) ;


INSERT INTO tipo_de_exercicio (codigo,nome,calorias_horas) VALUES (1,'futebol',760),(2,'basquete',584),(3,'corrida_obstaculo',715),(4,'golfe',315),(5,'volei',350),(6,'tenis',610),(7,'corrida',610),(8,'futebol americano',580),(9,'remo',470),(10,'caminhada',440); 

INSERT INTO USUARIO (rg,nome,idade,peso_inicial,sexo,altura) VALUES (12345,'Calebe',17,59,'M',1.71),(23456,'Davi',15,60,'M',1.75),(34567,'Alessandra',25,65,'F',1.82),(45678,'Rodolfo',22,71,'M',1.71),(56789,'Gustavo',33,82,'M',1.82),(67890,'Buteri',13,47,'M',1.73),(11234,'Maira',18,58,'F',1.91),(22345,'Rosilene',31,67,'F',1.55),(33456,'Felipe Noronha',27,62,'M',1.7),(44567,'Pedro',60,35,'M',1.61);


INSERT INTO TENIS (Codigo_tenis, Modelo, especialidade) VALUES (1010, 'Nike1v9', 'futebol'), (2020, 'Penalty', 'basquete'),(3030, 'Adidas3', 'volei'),(4040, 'Hypervenom', 'corrida'),(5050, 'Umbro', 'Golfe'),(6060, 'Puma', 'Corrida'),(7070, 'Umbro2', 'futebol'),(8080, 'Havaianas', 'futsal'),(9090, 'Nike', 'corrida'),(1212, 'Adidas2', 'Basquete');


INSERT INTO EXERCICIO(data_inicio,data_fim,latitude,longitude,horario_inicio,horario_fim,calorias_gastas,peso_atual,fk_tipo_de_exercicio_codigo,fk_usuario_rg,fk_sensor_codigo_sensor,fk_tenis_codigo_tenis) VALUES('2019-06-30','2019-06-30',-23.6506557,-46.5603576,'16:00','17:00',760,59,1,12345,4321,1010),('2019-07-01','2019-07-01',-19.9215223,-43.9340913,'17:00','18:00',584,60,2,23456,5432,2020),('2019-07-02','2019-07-02',34.0326511,-118.4602074,'18:00','19:00',715,65,3,34567,6543,3030),('2019-07-03','2019-07-03',33.8993738,-118.3787682,'19:00','20:00',315,71,4,45678,7654,4040),('2019-07-04','2019-07-04',37.4030185,-122.3212805,'20:00','21:00',350,82,5,56789,8765,5050),('2019-07-05','2019-07-05',24.3781314,-80.4603501,'21:00','22:00',610,47,6,67890,9876,6060),('2019-07-06','2019-07-06',22.3531176,113.8475127,'22:00','23:00',610,58,7,11234,1987,7070),('2019-07-07','2019-07-07',25.0000188,-71.0087548,'23:00','00:00',580,67,8,22345,2987,8080),('2019-07-08','2019-07-09',-25.7663566,-49.7417204,'00:00','01:00',470,62,9,33456,3987,9090),('2019-07-09','2019-07-09',43.7184038,-79.5181409,'01:00','02:00',440,35,10,44567,4874,1212);
  
  

## Marco de Entrega 08 em: (29/05/2019)<br>


### 9	TABELAS E PRINCIPAIS CONSULTAS<br>
    OBS: Incluir para cada tópico as instruções SQL + imagens (print da tela) mostrando os resultados.<br>
#### 9.1	CONSULTAS DAS TABELAS COM TODOS OS DADOS INSERIDOS (Todas) <br>
#### 9.2	CONSULTAS DAS TABELAS COM FILTROS WHERE (Mínimo 4)<br>
#### 9.3	CONSULTAS QUE USAM OPERADORES LÓGICOS, ARITMÉTICOS E TABELAS OU CAMPOS RENOMEADOS (Mínimo 11)
    a) Criar 5 consultas que envolvam os operadores lógicos AND, OR e Not
    b) Criar no mínimo 3 consultas com operadores aritméticos 
    c) Criar no mínimo 3 consultas com operação de renomear nomes de campos ou tabelas
#### 9.4	CONSULTAS QUE USAM OPERADORES LIKE E DATAS (Mínimo 12) <br>
    a) Criar outras 5 consultas que envolvam like ou ilike
    b) Criar uma consulta para cada tipo de função data apresentada.


    
#### 9.5	ATUALIZAÇÃO E EXCLUSÃO DE DADOS (Mínimo 6)<br>


#### 9.6	CONSULTAS COM JUNÇÃO E ORDENAÇÃO (Mínimo 6)<br>
        a) Uma junção que envolva todas as tabelas possuindo no mínimo 3 registros no resultado
        b) Outras junções que o grupo considere como sendo as de principal importância para o trabalho
        

### ATUALIZAÇÃO DA DOCUMENTAÇÃO DOS SLIDES PARA APRESENTAÇAO SEMESTRAL (Mínimo 6 e Máximo 10)<br>


#### 9.7	CONSULTAS COM GROUP BY E FUNÇÕES DE AGRUPAMENTO (Mínimo 6)<br>

#### 9.8	CONSULTAS COM LEFT E RIGHT JOIN (Mínimo 4)<br>
#### 9.9	CONSULTAS COM SELF JOIN E VIEW (Mínimo 6)<br>
        a) Uma junção que envolva Self Join
        b) Outras junções com views que o grupo considere como sendo de relevante importância para o trabalho
#### 9.10	SUBCONSULTAS (Mínimo 3)<br>

#### 9.11	LISTA DE CODIGOS DAS FUNÇÕES E TRIGGERS<br>
        Detalhamento sobre funcionalidade de cada código.
        a) Objetivo
        b) Código do objeto (função/trigger)
        c) exemplo de dados para aplicação
        d) resultados em forma de tabela/imagem
<br>


#### 9.12	GERACAO DE DADOS (MÍNIMO DE 100 MIL REGISTROS PARA PRINCIPAL RELAÇAO)<br>
        a) principal tabela do sistema deve ter no mínimo 100 mil registros
        b) tabelas diretamente relacionadas a tabela principal 10 mil registros
        c) tabelas auxiliares de relacao multivalorada mínimo de 10 registros
        d) registrar o tempo de inserção em cada uma das tabelas do banco de dados
        e) especificar a quantidade de registros inseridos em cada tabela
        Para melhor compreensão verifiquem o exemplo na base de testes:<br>
        https://github.com/discipbd2/base-de-testes-locadora
        

#### 9.13	Backup do Banco de Dados<br>
        Detalhamento do backup.
        a) Tempo
        b) Tamanho
        c) Teste de restauração (backup)
        d) Tempo para restauração
        e) Teste de restauração (script sql)
        f) Tempo para restauração (script sql)
<br>

Data de Entrega: (Data a ser definida)
<br>

#### 9.14	APLICAÇAO DE ÍNDICES E TESTES DE PERFORMANCE<br>
    a) Lista de índices, tipos de índices com explicação de porque foram implementados nas consultas 
    b) Performance esperada VS Resultados obtidos
    c) Tabela de resultados comparando velocidades antes e depois da aplicação dos índices (constando velocidade esperada com planejamento, sem indice e com índice Vs velocidade de execucao real com índice e sem índice).
    d) Escolher as consultas mais complexas para serem analisadas (consultas com menos de 2 joins não serão aceitas)
    e) As imagens do Explain devem ser inclusas no trabalho, bem como explicações sobre os resultados obtidos.
    f) Inclusão de tabela mostrando as 10 execuções, excluindo-se o maior e menor tempos para cada consulta e 
    obtendo-se a media dos outros valores como resultado médio final.
<br>
    Data de Entrega: (Data a ser definida)
<br>   

### 10	ATUALIZAÇÃO DA DOCUMENTAÇÃO DOS SLIDES PARA APRESENTAÇAO FINAL (Mínimo 6 e Máximo 10)<br>
<br>
    Data de Entrega: (Data a ser definida)
<br>

### 11 Backup completo do banco de dados postgres 
    a) deve ser realizado no formato "backup" 
        (Em Dump Options #1 Habilitar opções Don't Save Owner e Privilege)
    b) antes de postar o arquivo no git o mesmo deve ser testado/restaurado por outro grupo de alunos/dupla
    c) informar aqui o grupo de alunos/dupla que realizou o teste.

    
### 12	TUTORIAL COMPLETO DE PASSOS PARA RESTAURACAO DO BANCO E EXECUCAO DE PROCEDIMENTOS ENVOLVIDOS NO TRABALHO PARA OBTENÇÃO DOS RESULTADOS<br>
        a) Outros grupos deverão ser capazes de restaurar o banco 
        b) executar todas as consultas presentes no trabalho
        c) executar códigos que tenham sido construídos para o trabalho 
        d) realizar qualquer procedimento executado pelo grupo que desenvolveu o trabalho

### 13	DIFICULDADES ENCONTRADAS PELO GRUPO<br>  

    
Data de Entrega final: (Data a ser definida)
<br>

       
### 14  FORMATACAO NO GIT: https://help.github.com/articles/basic-writing-and-formatting-syntax/
<comentario no git>
    
##### About Formatting
    https://help.github.com/articles/about-writing-and-formatting-on-github/
    
##### Basic Formatting in Git
    
    https://help.github.com/articles/basic-writing-and-formatting-syntax/#referencing-issues-and-pull-requests
   
    
##### Working with advanced formatting
    https://help.github.com/articles/working-with-advanced-formatting/

#### Mastering Markdown
    https://guides.github.com/features/mastering-markdown/

### OBSERVAÇÕES IMPORTANTES

#### Todos os arquivos que fazem parte do projeto (Imagens, pdfs, arquivos fonte, etc..), devem estar presentes no GIT. Os arquivos do projeto vigente não devem ser armazenados em quaisquer outras plataformas.
1. Caso existam arquivos com conteúdos sigilosos, comunicar o professor que definirá em conjunto com o grupo a melhor forma de armazenamento do arquivo.

#### Todos os grupos deverão fazer Fork deste repositório e dar permissões administrativas ao usuário deste GIT, para acompanhamento do trabalho.

#### Os usuários criados no GIT devem possuir o nome de identificação do aluno (não serão aceitos nomes como Eu123, meuprojeto, pro456, etc). Em caso de dúvida comunicar o professor.


Link para BrModelo:<br>
http://sis4.com/brModelo/brModelo/download.html
<br>


Link para curso de GIT<br>
![https://www.youtube.com/curso_git](https://www.youtube.com/playlist?list=PLo7sFyCeiGUdIyEmHdfbuD2eR4XPDqnN2?raw=true "Title")


        
       

    





