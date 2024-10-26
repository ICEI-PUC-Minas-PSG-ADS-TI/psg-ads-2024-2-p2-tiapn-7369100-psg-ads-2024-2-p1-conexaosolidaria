## 4. Projeto da Solução

<span style="color:red">Pré-requisitos: <a href="03-Modelagem do Processo de Negocio.md"> Modelagem do Processo de Negocio</a></span>

## 4.1. Arquitetura da solução

 **Diagrama de Arquitetura**:
 
 ![Exemplo de Arquitetura](./images/geral.jpg)
 

### 4.2. Protótipos de telas

Visão geral da interação do usuário pelas telas do sistema e protótipo interativo das telas com as funcionalidades que fazem parte do sistema.

![Exemplo de Wireframe](images/telas/tela1.png)
![Exemplo de Wireframe](images/telas/tela2.png)
![Exemplo de Wireframe](images/telas/tela3.png)
![Exemplo de Wireframe](images/telas/tela4.png)
![Exemplo de Wireframe](images/telas/tela5.png)
![Exemplo de Wireframe](images/telas/tela6.png)
![Exemplo de Wireframe](images/telas/tela7.png)
![Exemplo de Wireframe](images/telas/tela8.png)
![Exemplo de Wireframe](images/telas/tela9.png)
![Exemplo de Wireframe](images/telas/tela10.png)
![Exemplo de Wireframe](images/telas/tela11.png)
![Exemplo de Wireframe](images/telas/tela12.png)

### 4.3. Modelo de dados

O desenvolvimento da solução proposta requer a existência de bases de dados que permitam efetuar os cadastros de dados e controles associados aos processos identificados, assim como recuperações.

#### 4.3.1 Modelo ER

O Modelo ER representa através de um diagrama como as entidades (coisas, objetos) se relacionam entre si na aplicação interativa.]

As referências abaixo irão auxiliá-lo na geração do artefato “Modelo ER”.

![Como fazer um diagrama entidade relacionamento | Lucidchart](images/DER.jpg)

#### 4.3.2 Esquema Relacional

O Esquema Relacional corresponde à representação dos dados em tabelas juntamente com as restrições de integridade e chave primária.
 
As referências abaixo irão auxiliá-lo na geração do artefato “Esquema Relacional”.

> - [Criando um modelo relacional - Documentação da IBM](https://www.ibm.com/docs/pt-br/cognos-analytics/10.2.2?topic=designer-creating-relational-model)

![Exemplo de um modelo relacional](images/logico.jpg "Exemplo de Modelo Relacional.")
---


#### 4.3.3 Modelo Físico

<code>

 CREATE TABLE Voluntario (
    ID_Voluntario INT PRIMARY KEY,
    Nome VARCHAR,
    CPF INT,
    fk_Telefone_Telefone_PK VARCHAR,
    Endereco_ VARCHAR,
    CEP VARCHAR,
    Data_Nascimento_ DATE,
    E_mail VARCHAR,
    Senha VARCHAR,
    Profissao VARCHAR,
    Descricao_Pessoal_ VARCHAR,
    Formacao_Academica VARCHAR
);

CREATE TABLE ONG (
    ID_ONG INT PRIMARY KEY,
    Nome VARCHAR,
    CNPJ VARCHAR,
    Endreco VARCHAR,
    FK_Telefone_Telefone_PK VARCHAR,
    FK_Area_Atuacao_Area_Atuacao_PK VARCHAR,
    Historico VARCHAR,
    FK_Necessidades_Necessidades_PK VARCHAR,
    E_mail VARCHAR,
    Senha VARCHAR
);

CREATE TABLE Chat (
    ID_Chat INT,
    Mensagem VARCHAR,
    Data_Hora DATE
);

CREATE TABLE Match_Demonstra_Interesse (
    ID_Match INT PRIMARY KEY,
    Data_Match DATE,
    fk_Voluntario_ID_Voluntario INT,
    fk_ONG_ID_ONG INT
);

CREATE TABLE Telefone (
    Telefone_PK VARCHAR NOT NULL PRIMARY KEY,
    Telefone VARCHAR
);

CREATE TABLE Telefone (
    Telefone_PK VARCHAR NOT NULL PRIMARY KEY,
    Telefone VARCHAR
);

CREATE TABLE Area_Atuacao_ (
    Area_Atuacao__PK VARCHAR NOT NULL PRIMARY KEY,
    Area_Atuacao_ VARCHAR
);

CREATE TABLE Necessidades (
    Necessidades_PK VARCHAR NOT NULL PRIMARY KEY,
    Necessidades VARCHAR
);
 
ALTER TABLE Voluntario ADD CONSTRAINT FK_Voluntario_2
    FOREIGN KEY (fk_Telefone_Telefone_PK)
    REFERENCES Telefone (Telefone_PK)
    ON DELETE NO ACTION;
 
ALTER TABLE ONG ADD CONSTRAINT FK_ONG_2
    FOREIGN KEY (FK_Telefone_Telefone_PK)
    REFERENCES Telefone (Telefone_PK)
    ON DELETE NO ACTION;
 
ALTER TABLE ONG ADD CONSTRAINT FK_ONG_3
    FOREIGN KEY (FK_Area_Atuacao_Area_Atuacao_PK)
    REFERENCES Area_Atuacao_ (Area_Atuacao__PK)
    ON DELETE NO ACTION;
 
ALTER TABLE ONG ADD CONSTRAINT FK_ONG_4
    FOREIGN KEY (FK_Necessidades_Necessidades_PK)
    REFERENCES Necessidades (Necessidades_PK)
    ON DELETE NO ACTION;
 
ALTER TABLE Match_Demonstra_Interesse ADD CONSTRAINT FK_Match_Demonstra_Interesse_2
    FOREIGN KEY (fk_Voluntario_ID_Voluntario)
    REFERENCES Voluntario (ID_Voluntario);
 
ALTER TABLE Match_Demonstra_Interesse ADD CONSTRAINT FK_Match_Demonstra_Interesse_3
    FOREIGN KEY (fk_ONG_ID_ONG)
    REFERENCES ONG (ID_ONG);

</code>

### 4.4. Tecnologias

| **Dimensão**   | **Tecnologia**  |
| ---            | ---             |
| SGBD           | MySQL           |
| Front end      | HTML+CSS+JS+Bootstrap |
| Back end       | C# |
| Deploy         | Github Pages |
| IDE            | Visual Studio Code e Visual Studio |

