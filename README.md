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
  


*Relatório que informe o desempenho do usuário após a atividade física incluindo as calorias gastas, distância percorrida e o tempo gasto. 



*Relatório que informe o progresso do peso do usuário de acordo com sua meta mensal



*Relatório que informe o progresso da altura do usuário



*Relatorio que informe as calorias que faltam para o usuário atingir sua meta



*Relatório que informe os exercicios mais apropriados para o usuário cumprir a meta

## Marco de Entrega 03 em: (13/05/2019)<br>

#### 4.2 TABELA DE DADOS DO SISTEMA:
    a) Esta tabela deve conter todos os atributos do sistema e um mínimo de 10 linhas/registros de dados.
    b) Esta tabela tem a intenção de simular um relatório com todos os dados que serão armazenados 
    e deve ser criada antes do modelo conceitual
    c) Após criada esta tabela não deve ser modificada, pois será comparada com os resultados finais na conclusão do trabalho
    
    
    
    
    
    
    
  (https://github.com/Trabalhomoisestenis/trabalho01/blob/master/shoestabela.ods)

## Marco de Entrega 04 em: (15/05/2019)<br>

### 5.MODELO CONCEITUAL<br>
    A) NOTACAO ENTIDADE RELACIONAMENTO 
        * Para nosso prótótipo limitaremos o modelo conceitual nas 5 principais entidades do escopo
        * O protótipo deve possui no mínimo duas relações N para N
        * o mínimo de entidades do modelo conceitual será igual a 5
        
![Alt text](https://github.com/Trabalhomoisestenis/trabalho01/blob/master/birinha.png)
    B) QUALIDADE 
        Garantir que a semântica dos atributos seja clara no esquema
        Criar o esquema de forma a garantir a redução de informação redundante, possibilidade de valores null, 
        e tuplas falsas
    
        
    
#### 5.1 Validação do Modelo Conceitual
    [Grupo01]: [Nomes dos que participaram na avaliação]
    [Grupo02]: [Nomes dos que participaram na avaliação]
    
## Marco de Entrega 05 em: (20/05/2019)<br>

#### 5.2 DESCRIÇÃO DOS DADOS 

   PESO: Tabela que armazena as informações relativas ao peso do usuário ao longo do tempo.
   	
	Codigo_peso: campo que armazena o código do peso registrado.
	
	Peso: campo que armazena o peso registrado pelo usuário.
	
	Data_registro: Data do armazenamento do peso.




   Altura: Tabela que armazena as informações relativas a altura do usuário ao longo do tempo.
   	
	Codigo_altura: campo que armazena o código da altura registrada.
	
	Altura: campo que armazena a altura registrada pelo usuário.
	
	Data_registro: Data do armazenamento da altura.
	
	
   USUÁRIO: Tabela que armazena as informações relativas ao usuário.

	RG: Campo que armazena o número do Registro Geral de cada usuário.
	
	Nome: Campo que armazena o nome do usuário.

	Data_nascimento: Campo que armazena a data de nascimento do usuário.

	Sexo: Campo que armazena o sexo do usuário.
	



TÊNIS: Tabela que armazena as informações relativas ao tênis adquirido pelo usuário.	
	
	Código_Tênis: Campo que armazena o código específico de um tênis.

	Modelo: Campo que armazena o modelo do tênis.

	
ESPECIALIDADE_TENIS: Tabela que armazena as informações relativas a especialidade de cada modelo de tênis.
	
	codigo_especialidade: campo que armazena o código da especialidade do tênis.
	
	nome_especialidade: campo que armazena o nome da especialidade do tênis.




SENSOR: Tabela que armazena as informações relativas ao sensor adquirido pelo usuário:

	Código_Sensor: Campo que armazena o código do sensor.
	
	

Tipo de Exercícios: Tabela que armazena as informações relativas a cada exercício:

	Nome: Campo que armazena o nome do exercício

	Calorias_gastas_hora: Campo que armazena a quantidade de calorias gastas por hora 
	que aquele exercício específico promove 
	
	Código: Campo que armazena o código do exercício


EXERCÍCIO: Tabela que armazena as informações do usuário/tipo_de_exercício/tênis/sensor durante a prática de uma atividade.

	Data: Data do início da prática da atividade.
	
	Latitude: Coordenada de localização da posição do usuário ao longo do exercício.
	
	Longitude: Coordenada de localização da posição do usuário ao longo do exercício.
	
	Tempo: Contagem do tempo que o usuário gastou para realizar o exercício.
	
	
Endereço:Tabela que armazena o cep do usuario. 	
	
	cep: Campo que armazena o cep do usuario
	
	
Município : Tabela que armazena as informações relativas ao município do usuário.
	
	id: Campo que armazena o id do município	
	
	nome: Campo que armazena o nome do município
	
Estado : Tabela que armazena as informações relativas ao Estado do usuário.

	id: Campo que armazena o id do Estado	
	
	nome: Campo que armazena o nome do Estado
	
Bairro: Tabela que armazena as informações relativas ao Bairro do usuário.

	id: Campo que armazena o id do Bairro	
	
	nome: Campo que armazena o nome do Bairro


																				
  
## Marco de Entrega 06 em: (22/05/2019)<br>

### 6	MODELO LÓGICO<br>
![Alt text](https://github.com/Trabalhomoisestenis/trabalho01/blob/master/tonga.png)
### 7	MODELO FÍSICO<br>
       
/* Lógico_1: */
jj

CREATE TABLE Usuario (
    RG int PRIMARY KEY,
    Nome varchar(100),
    Data_nascimento Date,
    Sexo char(1)
);

CREATE TABLE Tenis (
    Codigo_Tenis int PRIMARY KEY,
    Modelo varchar(40),
    fk_especialidade_tenis_Codigo_espcialidade int
);

CREATE TABLE Sensor (
    Codigo_Sensor int PRIMARY KEY
);

CREATE TABLE tipo_de_exercicio (
    Nome varchar(40),
    Calorias_gastas_por_hora float,
    Codigo int PRIMARY KEY
);

CREATE TABLE Exercicio (
    Data date,
    Latitude float,
    Longitude float,
    tempo time,
    fk_tipo_de_exercicio_Codigo int,
    fk_Usuario_RG int,
    fk_Sensor_Codigo_Sensor int,
    fk_Tenis_Codigo_Tenis int
);

CREATE TABLE especialidade_tenis (
    Nome_especialidade varchar(100),
    Codigo_espcialidade int PRIMARY KEY
);

CREATE TABLE Pesos_usuarios (
    Peso float,
    data_registro date,
    Codigo_peso int PRIMARY KEY,
    fk_Usuario_RG int
);

CREATE TABLE Altura_usuarios (
    data_registro date,
    Altura float,
    codigo_altura int PRIMARY KEY,
    fk_Usuario_RG int
);

CREATE TABLE Meta_mensal_usuario (
    Calorias float,
    Codigo_meta int PRIMARY KEY,
    data_registro Date,
    fk_Usuario_RG int
);

CREATE TABLE Endereco (
    cep int PRIMARY KEY,
    fk_Usuario_RG int,
    fk_Bairro_Id int,
    fk_Municipio_id int,
    fk_Estado_id int
);

CREATE TABLE Estado (
    id int PRIMARY KEY,
    Nome varchar(100)
);

CREATE TABLE Municipio (
    id int PRIMARY KEY,
    Nome varchar(100)
);

CREATE TABLE Bairro (
    Id int PRIMARY KEY,
    Nome varchar(100)
);
 
ALTER TABLE Tenis ADD CONSTRAINT FK_Tenis_2
    FOREIGN KEY (fk_especialidade_tenis_Codigo_espcialidade)
    REFERENCES especialidade_tenis (Codigo_espcialidade)
    ON DELETE RESTRICT;
 
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
 
ALTER TABLE Pesos_usuarios ADD CONSTRAINT FK_Pesos_usuarios_2
    FOREIGN KEY (fk_Usuario_RG)
    REFERENCES Usuario (RG)
    ON DELETE RESTRICT;
 
ALTER TABLE Altura_usuarios ADD CONSTRAINT FK_Altura_usuarios_2
    FOREIGN KEY (fk_Usuario_RG)
    REFERENCES Usuario (RG)
    ON DELETE RESTRICT;
 
ALTER TABLE Meta_mensal_usuario ADD CONSTRAINT FK_Meta_mensal_usuario_2
    FOREIGN KEY (fk_Usuario_RG)
    REFERENCES Usuario (RG)
    ON DELETE RESTRICT;
 
ALTER TABLE Endereco ADD CONSTRAINT FK_Endereco_2
    FOREIGN KEY (fk_Usuario_RG)
    REFERENCES Usuario (RG)
    ON DELETE CASCADE;
 
ALTER TABLE Endereco ADD CONSTRAINT FK_Endereco_3
    FOREIGN KEY (fk_Bairro_Id)
    REFERENCES Bairro (Id)
    ON DELETE CASCADE;
 
ALTER TABLE Endereco ADD CONSTRAINT FK_Endereco_4
    FOREIGN KEY (fk_Municipio_id)
    REFERENCES Municipio (id)
    ON DELETE CASCADE;
 
ALTER TABLE Endereco ADD CONSTRAINT FK_Endereco_5
    FOREIGN KEY (fk_Estado_id)
    REFERENCES Estado (id)
    ON DELETE CASCADE;
## Marco de Entrega 07 em: (27/05/2019)<br>

### 8	INSERT APLICADO NAS TABELAS DO BANCO DE DADOS<br>
#### 8.1 DETALHAMENTO DAS INFORMAÇÕES

https://github.com/Trabalhomoisestenis/trabalho01/blob/master/querovedapau.ipynb


#### 8.2 INCLUSÃO DO SCRIPT PARA CRIAÇÃO DE TABELA E INSERÇÃO DOS DADOS 



CREATE TABLE Usuario (
    RG int PRIMARY KEY,
    Nome varchar(100),
    Data_nascimento Date,
    Sexo char(1)
);

CREATE TABLE Tenis (
    Codigo_Tenis int PRIMARY KEY,
    Modelo varchar(40),
    fk_especialidade_tenis_Codigo_espcialidade int
);

CREATE TABLE Sensor (
    Codigo_Sensor int PRIMARY KEY
);

CREATE TABLE tipo_de_exercicio (
    Nome varchar(40),
    Calorias_gastas_por_hora float,
    Codigo int PRIMARY KEY
);

CREATE TABLE Exercicio (
    Data date,
    Latitude float,
    Longitude float,
    tempo time,
    fk_tipo_de_exercicio_Codigo int,
    fk_Usuario_RG int,
    fk_Sensor_Codigo_Sensor int,
    fk_Tenis_Codigo_Tenis int
);

CREATE TABLE especialidade_tenis (
    Nome_especialidade varchar(100),
    Codigo_espcialidade int PRIMARY KEY
);

CREATE TABLE Pesos_usuarios (
    Peso float,
    data_registro date,
    Codigo_peso int PRIMARY KEY,
    fk_Usuario_RG int
);

CREATE TABLE Altura_usuarios (
    data_registro date,
    Altura float,
    codigo_altura int PRIMARY KEY,
    fk_Usuario_RG int
);

CREATE TABLE Meta_mensal_usuario (
    Calorias float,
    Codigo_meta int PRIMARY KEY,
    data_registro Date,
    fk_Usuario_RG int
);

CREATE TABLE Endereco (
    cep int PRIMARY KEY,
    fk_Usuario_RG int,
    fk_Bairro_Id int,
    fk_Municipio_id int,
    fk_Estado_id int
);

CREATE TABLE Estado (
    id int PRIMARY KEY,
    Nome varchar(100)
);

CREATE TABLE Municipio (
    id int PRIMARY KEY,
    Nome varchar(100)
);

CREATE TABLE Bairro (
    Id int PRIMARY KEY,
    Nome varchar(100)
);
 
ALTER TABLE Tenis ADD CONSTRAINT FK_Tenis_2
    FOREIGN KEY (fk_especialidade_tenis_Codigo_espcialidade)
    REFERENCES especialidade_tenis (Codigo_espcialidade)
    ON DELETE RESTRICT;
 
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
 
ALTER TABLE Pesos_usuarios ADD CONSTRAINT FK_Pesos_usuarios_2
    FOREIGN KEY (fk_Usuario_RG)
    REFERENCES Usuario (RG)
    ON DELETE RESTRICT;
 
ALTER TABLE Altura_usuarios ADD CONSTRAINT FK_Altura_usuarios_2
    FOREIGN KEY (fk_Usuario_RG)
    REFERENCES Usuario (RG)
    ON DELETE RESTRICT;
 
ALTER TABLE Meta_mensal_usuario ADD CONSTRAINT FK_Meta_mensal_usuario_2
    FOREIGN KEY (fk_Usuario_RG)
    REFERENCES Usuario (RG)
    ON DELETE RESTRICT;
 
ALTER TABLE Endereco ADD CONSTRAINT FK_Endereco_2
    FOREIGN KEY (fk_Usuario_RG)
    REFERENCES Usuario (RG)
    ON DELETE CASCADE;
 
ALTER TABLE Endereco ADD CONSTRAINT FK_Endereco_3
    FOREIGN KEY (fk_Bairro_Id)
    REFERENCES Bairro (Id)
    ON DELETE CASCADE;
 
ALTER TABLE Endereco ADD CONSTRAINT FK_Endereco_4
    FOREIGN KEY (fk_Municipio_id)
    REFERENCES Municipio (id)
    ON DELETE CASCADE;
 
ALTER TABLE Endereco ADD CONSTRAINT FK_Endereco_5
    FOREIGN KEY (fk_Estado_id)
    REFERENCES Estado (id)
    ON DELETE CASCADE;
https://github.com/Trabalhomoisestenis/trabalho01/blob/master/querovedapau.ipynb
 
#### 8.3 INCLUSÃO DO SCRIPT PARA EXCLUSÃO DE TABELAS EXISTENTES, CRIAÇÃO DE TABELA NOVAS E INSERÇÃO DOS DADOS
   DROP TABLE exercicio;
   DROP TABLE usuario;
   DROP TABLE TENIS;
   DROP TABLE tipo_de_exercicio;
   DROP TABLE sensor;
   DROP TABLE ENDEREÇO
   DROP TABLE ESTADO
   DROP TABLE pesos_usuarios
   DROP TABLE Altura_usuarios
   DROP TABLE Municipios
   DROP TABLE Bairro
   DROP TABLE Meta_mensal_usuario
   
CREATE TABLE Usuario (
    RG int PRIMARY KEY,
    Nome varchar(100),
    Data_nascimento Date,
    Sexo char(1)
);

CREATE TABLE Tenis (
    Codigo_Tenis int PRIMARY KEY,
    Modelo varchar(40),
    fk_especialidade_tenis_Codigo_espcialidade int
);

CREATE TABLE Sensor (
    Codigo_Sensor int PRIMARY KEY
);

CREATE TABLE tipo_de_exercicio (
    Nome varchar(40),
    Calorias_gastas_por_hora float,
    Codigo int PRIMARY KEY
);

CREATE TABLE Exercicio (
    Data date,
    Latitude float,
    Longitude float,
    tempo time,
    fk_tipo_de_exercicio_Codigo int,
    fk_Usuario_RG int,
    fk_Sensor_Codigo_Sensor int,
    fk_Tenis_Codigo_Tenis int
);

CREATE TABLE especialidade_tenis (
    Nome_especialidade varchar(100),
    Codigo_espcialidade int PRIMARY KEY
);

CREATE TABLE Pesos_usuarios (
    Peso float,
    data_registro date,
    Codigo_peso int PRIMARY KEY,
    fk_Usuario_RG int
);

CREATE TABLE Altura_usuarios (
    data_registro date,
    Altura float,
    codigo_altura int PRIMARY KEY,
    fk_Usuario_RG int
);

CREATE TABLE Meta_mensal_usuario (
    Calorias float,
    Codigo_meta int PRIMARY KEY,
    data_registro Date,
    fk_Usuario_RG int
);

CREATE TABLE Endereco (
    cep int PRIMARY KEY,
    fk_Usuario_RG int,
    fk_Bairro_Id int,
    fk_Municipio_id int,
    fk_Estado_id int
);

CREATE TABLE Estado (
    id int PRIMARY KEY,
    Nome varchar(100)
);

CREATE TABLE Municipio (
    id int PRIMARY KEY,
    Nome varchar(100)
);

CREATE TABLE Bairro (
    Id int PRIMARY KEY,
    Nome varchar(100)
);
 
ALTER TABLE Tenis ADD CONSTRAINT FK_Tenis_2
    FOREIGN KEY (fk_especialidade_tenis_Codigo_espcialidade)
    REFERENCES especialidade_tenis (Codigo_espcialidade)
    ON DELETE RESTRICT;
 
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
 
ALTER TABLE Pesos_usuarios ADD CONSTRAINT FK_Pesos_usuarios_2
    FOREIGN KEY (fk_Usuario_RG)
    REFERENCES Usuario (RG)
    ON DELETE RESTRICT;
 
ALTER TABLE Altura_usuarios ADD CONSTRAINT FK_Altura_usuarios_2
    FOREIGN KEY (fk_Usuario_RG)
    REFERENCES Usuario (RG)
    ON DELETE RESTRICT;
 
ALTER TABLE Meta_mensal_usuario ADD CONSTRAINT FK_Meta_mensal_usuario_2
    FOREIGN KEY (fk_Usuario_RG)
    REFERENCES Usuario (RG)
    ON DELETE RESTRICT;
 
ALTER TABLE Endereco ADD CONSTRAINT FK_Endereco_2
    FOREIGN KEY (fk_Usuario_RG)
    REFERENCES Usuario (RG)
    ON DELETE CASCADE;
 
ALTER TABLE Endereco ADD CONSTRAINT FK_Endereco_3
    FOREIGN KEY (fk_Bairro_Id)
    REFERENCES Bairro (Id)
    ON DELETE CASCADE;
 
ALTER TABLE Endereco ADD CONSTRAINT FK_Endereco_4
    FOREIGN KEY (fk_Municipio_id)
    REFERENCES Municipio (id)
    ON DELETE CASCADE;
 
ALTER TABLE Endereco ADD CONSTRAINT FK_Endereco_5
    FOREIGN KEY (fk_Estado_id)
    REFERENCES Estado (id)
    ON DELETE CASCADE;
https://github.com/Trabalhomoisestenis/trabalho01/blob/master/querovedapau.ipynb
 
  

## Marco de Entrega 08 em: (29/05/2019)<br>


### 9	TABELAS E PRINCIPAIS CONSULTAS<br>
    OBS: Incluir para cada tópico as instruções SQL + imagens (print da tela) mostrando os resultados.<br>
#### 9.1	CONSULTAS DAS TABELAS COM TODOS OS DADOS INSERIDOS (Todas) <br>
#### 9.2	CONSULTAS DAS TABELAS COM FILTROS WHERE (Mínimo 4)<br>
https://github.com/Trabalhomoisestenis/trabalho01/blob/master/consultawhere.png
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


        
       

    





