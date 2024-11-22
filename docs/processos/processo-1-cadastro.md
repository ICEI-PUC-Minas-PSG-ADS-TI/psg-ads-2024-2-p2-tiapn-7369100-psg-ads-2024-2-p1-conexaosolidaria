### 3.3.1 Processo 1 – CADASTRO E LOGIN DE ONGS E VOLUNTARIOS

Trata-se da tela de cadastro e login de ONGs e voluntários

![PROCESSO 1](../images/modelagem/cadastro.png "Modelo BPMN do Processo 1.")

#### Detalhamento das atividades

#### Para Voluntários:
Acesso ao Formulário de Cadastro: O voluntário clica em "Cadastrar-se" e é direcionado para o formulário de cadastro.
Preenchimento de Dados Pessoais: O voluntário insere suas informações pessoais (nome, telefone, endereço, data de nascimento, CPF, CEP, e-mail e senha).
Revisão e Confirmação: O voluntário revisa os dados e confirma o cadastro.
#### Para ONGs:
Acesso ao Formulário de Cadastro: A ONG clica em "Cadastrar-se" e é direcionada para o formulário de cadastro.
Preenchimento de Dados da ONG: A ONG insere informações.
Necessidades da ONG: A ONG fornece informações sobre os tipos de voluntários que busca.
Histórico da ONG: Um campo para um breve histórico explicando seu propósito e atividades.
Revisão e Confirmação: A ONG revisa os dados e confirma o cadastro.

_Os tipos de dados a serem utilizados são:_

_* **Caixa de texto** - campo texto de uma linha_


# Cadastro de Voluntários

| **Campo**            | **Tipo**         | **Restrições**                 | **Valor Default**     |
|-----------------------|------------------|--------------------------------|-----------------------|
| Nome do voluntário    | Caixa de texto   | Máximo 30 caracteres           | Sem valor padrão      |
| Telefone              | Numérico         | Máximo 12 caracteres           | Sem valor padrão      |
| CPF                   | Numérico         | Máximo 14 caracteres           | Sem valor padrão      |
| Registro do Conselho  | Caixa de texto   | Sem restrições                 | Sem valor padrão      |
| Área de atuação       | Caixa de texto   | Sem restrições                 | Sem valor padrão      |
| Endereço              | Caixa de texto   | Máximo 100 caracteres          | Sem valor padrão      |
| Email                 | Caixa de texto   | Formato de e-mail válido       | Sem valor padrão      |
| Senha                 | Caixa de texto   | Mínimo 8 caracteres            | Sem valor padrão      |

| **Comandos**         | **Destino**                             | **Descrição**             |
|-----------------------|-----------------------------------------|---------------------------|
| Cadastrar Voluntário  | Enviar pop-up de confirmação de cadastro | Botão principal de cadastro |
| Cancelar              | Retornar para tela de login            | Botão para cancelar ação  |

---

# Cadastro de ONGs

| **Campo**            | **Tipo**         | **Restrições**                 | **Valor Default**     |
|-----------------------|------------------|--------------------------------|-----------------------|
| Nome da ONG           | Caixa de texto   | Máximo 30 caracteres           | Sem valor padrão      |
| Telefone              | Numérico         | Máximo 12 caracteres           | Sem valor padrão      |
| CNPJ                  | Numérico         | Máximo 18 caracteres           | Sem valor padrão      |
| Área de atuação       | Caixa de texto   | Sem restrições                 | Sem valor padrão      |
| Endereço              | Caixa de texto   | Máximo 100 caracteres          | Sem valor padrão      |
| Email                 | Caixa de texto   | Formato de e-mail válido       | Sem valor padrão      |
| Senha                 | Caixa de texto   | Mínimo 8 caracteres            | Sem valor padrão      |

| **Comandos**         | **Destino**                             | **Descrição**             |
|-----------------------|-----------------------------------------|---------------------------|
| Cadastrar ONG         | Enviar pop-up de confirmação de cadastro | Botão principal de cadastro |
| Cancelar              | Retornar para tela de login            | Botão para cancelar ação  |
