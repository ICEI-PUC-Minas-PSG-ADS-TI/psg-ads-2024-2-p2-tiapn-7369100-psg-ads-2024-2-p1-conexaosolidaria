### 3.3.2 Processo 3 – PESQUISA DE INTERESSES ENTRE ONGS E VOLUNTARIOS

Trata-se da pesquisa de interesses entre ONGs e voluntários

![PROCESSO 3](../images/modelagem/pesquisar.png "Modelo BPMN do Processo 3.")


#### Detalhamento das atividades

#### Para Voluntários
Acesso à Aba de Match: O sistema de match conecta o voluntário com a ONG de acordo com a base nas preferências e necessidades de cada um, facilitando o engajamento e a colaboração.
Visualização de ONGs: O voluntário visualiza uma lista de ONGs com descrições detalhadas (informações, descrições, imagens, etc).
#### Para ONGs:
Acesso à Aba de Match: O sistema de match conecta a ONG com o voluntário de acordo com a base nas preferências e necessidades de cada um, facilitando o engajamento e a colaboração.
Visualização de Voluntários: A ONG vê uma lista de voluntários que indicaram interesse em colaborar (informações, descrições, imagens, etc).

_Os tipos de dados a serem utilizados são:_

_* **Caixa de texto** - campo texto de uma linha_

# Pesquisar ONGs e Voluntários

| **Campo**    | **Tipo**       | **Restrições**           | **Valor Default**     |
|--------------|----------------|--------------------------|-----------------------|
| Pesquisar    | Caixa de Texto | Máximo 30 caracteres     | Sem valor padrão      |

| **Comandos**     | **Destino**                                      | **Descrição**                                     |
|------------------|--------------------------------------------------|-------------------------------------------------|
| Matching         | Encaminhar para página do catálogo de Voluntários | Ação principal para encontrar voluntários       |
| Card Voluntários | Encaminhar para página de perfil de Voluntários  | Visualizar detalhes do perfil de voluntários    |

---

# Pesquisar Voluntários

| **Campo**    | **Tipo**       | **Restrições**           | **Valor Default**     |
|--------------|----------------|--------------------------|-----------------------|
| Pesquisar    | Caixa de Texto | Máximo 30 caracteres     | Sem valor padrão      |

| **Comandos**     | **Destino**                                      | **Descrição**                                     |
|------------------|--------------------------------------------------|-------------------------------------------------|
| Matching         | Encaminhar para página do catálogo de ONGs       | Ação principal para encontrar ONGs              |
| Card ONGs        | Encaminhar para página de perfil de ONGs         | Visualizar detalhes do perfil de ONGs           |
