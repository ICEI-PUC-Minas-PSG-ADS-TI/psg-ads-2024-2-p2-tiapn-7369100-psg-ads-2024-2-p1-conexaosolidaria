## 3. Modelagem dos Processos de Negócio

> **Links Úteis**:
> - [Modelagem de Processos AS-IS x TO-BE](https://dheka.com.br/modelagem-as-is-to-be/)
> - [20 Dicas Práticas de Modelagem de Processos](https://dheka.com.br/20-dicas-praticas-de-modelagem-de-processos/)

### 3.1. Modelagem da situação atual (Modelagem AS IS)

_Apresente uma descrição textual de como os sistemas atuais resolvem o problema que se propõe a resolver.  Caso sua proposta seja inovadora e não existam processos claramente definidos, **apresente como as tarefas que o seu sistema pretende implementar são executadas atualmente**, mesmo que não se utilize tecnologia computacional._

Com o tema do projeto definido, escolham alguns processos neste contexto de negócios. Para ilustrar potenciais ganhos com a automatização, imaginem processos manuais, ineficientes e/ou com muitas idas e vindas, gerando, assim, retrabalho.
Colem aqui os modelos dos processos atuais (modelo AS-IS), elaborados com o apoio da ferramenta baseada em BPMN utilizada na disciplina.

### 3.2. Descrição geral da proposta (Modelagem TO BE)

## A) Cadastro

### Para Voluntários:
1. **Acesso ao Formulário de Cadastro**: O voluntário clica em "Cadastrar-se" e é direcionado para o formulário de cadastro.
2. **Preenchimento de Dados Pessoais**: O voluntário insere suas informações pessoais (nome, telefone, endereço, data de nascimento, CPF, CEP, e-mail e senha).
3. **Revisão e Confirmação**: O voluntário revisa os dados preenchidos e confirma o cadastro.

### Para ONGs:
1. **Acesso ao Formulário de Cadastro**: A ONG clica em "Cadastrar-se" e é direcionada para o formulário de cadastro.
2. **Preenchimento de Dados da ONG**: A ONG insere informações institucionais, como nome, endereço, e-mail e telefone.
3. **Necessidades da ONG**: A ONG fornece informações sobre os tipos de voluntários que está buscando e suas qualificações.
4. **Histórico da ONG**: Um campo para a ONG inserir um breve histórico explicando seu propósito e as atividades realizadas.
5. **Revisão e Confirmação**: A ONG revisa os dados e confirma o cadastro.

## B) Pesquisar

### Para Voluntários:
1. **Acesso à Aba de Match**: O voluntário navega para a aba de match.
2. **Visualização de ONGs**: O voluntário visualiza uma lista de ONGs, com descrições detalhadas sobre suas atividades, localização e necessidades.

### Para ONGs:
1. **Acesso à Aba de Match**: A ONG navega para a aba de match.
2. **Visualização de Voluntários**: A ONG visualiza uma lista de voluntários que demonstraram interesse em colaborar, com descrições sobre suas qualificações e disponibilidade.

---

## C) Sistema de Match

### Para Voluntários:
1. **Indicação de Interesse**: O voluntário clica no ícone de coração para indicar interesse em uma ONG.
2. **Notificação para a ONG**: A ONG recebe uma notificação sobre o interesse do voluntário.
3. **Ativação do Chat**: Se a ONG aceitar o interesse, o chat é ativado para comunicação.

### Para ONGs:
1. **Indicação de Interesse**: A ONG clica no ícone de coração para indicar interesse em um voluntário.
2. **Notificação para o Voluntário**: O voluntário recebe uma notificação sobre o interesse da ONG.
3. **Ativação do Chat**: Se o voluntário também der match, o chat é ativado para discutir a colaboração.

### 3.3. Modelagem dos processos

[PROCESSO 1 - Cadastro](./processos/processo-1-cadastro.md "Trata-se da tela de cadastro e login de ONGs e voluntários.")

[PROCESSO 2 - Pesquisar](./processos/processo-2-sistema-match.md "Trata-se da tela de Match d ONGs e voluntários.")

[PROCESSO 3 - Sistema de Match](./processos/processo-3-pesquisar.md "Trata-se da pesquisa de interesses entre ONGs e voluntários.")
