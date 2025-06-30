# Relatório de Bugs

**Software:** SwagLabs
**QA responsável:** Victor Nadoti
**Data:** 12.05.25


### 🐞 **Bug 01: Campo de Pesquisa**

| **ID**     | **Descrição**                                                                                                                                             |
| ---------- | --------------------------------------------------------------------------------------------------------------------------------------------------------- |
| BUG-001    | Após um login efetuado com sucesso, ao ser redirecionado para a página principal da aplicação, não foi encontrado em nenhum local da página um campo de busca para produto. |

| **Severidade do Bug** | **Prioridade de Correção** | **Status** |
| :-------------------: | :------------------------: | :--------: |
|         Média         |            Média            |   Aberto   |

| **Passo a passo para simular o bug**                           |
| -------------------------------------------------------------- |
| 1. Login na Aplicação                                          |
| 2. Procurar por campo de pesquisa                              |


|                        **Comportamento Esperado**                       |                        **Comportamento Obtido**                        |
| :---------------------------------------------------------------------: | :--------------------------------------------------------------------: |
| A Página deveria conter um campo de busca para a pesquisa e assim facilitar o usuário a encontrar produtos. | Não foi encontrado em nenhum local da página um campo de busca para auxiliar o usuário a encontrar produtos. |

| **Ambiente**             |
| ------------------------ |
| Ambiente de homologação. |
| Desktop com Windows 11.  |
| Google Chrome 138.0.7204.50    |
| Swaglabs           |

| **Funcionalidade Afetada** |        **Caso de Teste Relacionado**       |
| :------------------------: | :----------------------------------------: |
| - | - |

|                **Evidência(s)**               |
| :-------------------------------------------: |
| ![Home](https://github.com/vnadoti/manual-test-swaglabs/evidencias/home-page.gif) |

___ 

### 🐞 **Bug 02: Manipular Quantidade no Carrinho de Compras **

| **ID**     | **Descrição**                                                                                                                                             |
| ---------- | --------------------------------------------------------------------------------------------------------------------------------------------------------- |
| BUG-002    | Após a adição de um produto no carrinho de compras, não foi encontrado em nenhum local da página um botão para manipular a quantiade de itens para o produto (+ ou  -). |

| **Severidade do Bug** | **Prioridade de Correção** | **Status** |
| :-------------------: | :------------------------: | :--------: |
|         Média         |            Média           |   Aberto   |

| **Passo a passo para simular o bug**                           |
| -------------------------------------------------------------- |
| 1. Usuário está na página do carrinho com um item (Qtd: 1)     |                                   
| 2. Procurar por campo de para aumentar ou diminuir produto     |


|                        **Comportamento Esperado**                       |                        **Comportamento Obtido**                        |
| :---------------------------------------------------------------------: | :--------------------------------------------------------------------: |
| Campo para adiconar ou remover a quantidade de produtos  | Não existe um campo para adicionar ou remover a quantidade de produtos| 


| **Ambiente**             |
| ------------------------ |
| Ambiente de homologação. |
| Desktop com Windows 11.  |
| Google Chrome 138.0.7204.50    |
| Swaglabs           |

| **Funcionalidade Afetada** |        **Caso de Teste Relacionado**       |
| :------------------------: | :----------------------------------------: |
| Adicionar produto | TC-006 - Adicionar Produtos ao carrinho |
| Remover produto | TC-007 - Remover Produtos ao carrinho |

|                **Evidência(s)**               |
| :-------------------------------------------: |
| ![Quantidade](https://github.com/vnadoti/manual-test-swaglabs/evidencias/qtdade.gif)|









