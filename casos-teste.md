
### 🔐Login Válido
| ID                     | Descrição                                                             |
| :--------------------- | :-------------------------------------------------------------------- |
| TC-001 | Verifique se um usuário registrado consegue efetuar login com sucesso. |

| **Pré-condições**                            |
| :------------------------------------------- |
| Usuário com conta válida existente. |

| **Passos**                                                                    |
| :---------------------------------------------------------------------------- |
| **DADO** que o usuário está na página de login (https://www.saucedemo.com/v1/index.html)     |
| **QUANDO** ele insere o username cadastrado e a senha correta                   |
| **E** clica no botão "login"                                                  |
| **ENTÃO** ele deve ser redirecionado para a página inicial da aplicação (ou homepage) |
| **E** o nome do usuário ou uma saudação deve ser visível                      |                                                               |

| **Critérios de aceitação**                                                                            |
| :---------------------------------------------------------------------------------------------------- |
| O sistema deve redirecionar corretamente para a página inicial da aplicação |


| **Evidência:** | 
| :---------------------------------------------------------------------------------------------------- |
|![Login com sucesso](https://github.com/vnadoti/manual-test-swaglabs/blob/main/evidencias/login.gif)|

___

### 🔐Login com senha inválida
| ID                     | Descrição                                                             |
| :--------------------- | :-------------------------------------------------------------------- |
| TC-002 | Verifique se um usuário com password inválido consegue efetuar login com sucesso . |

| **Pré-condições**                            |
| :------------------------------------------- |
| Usuário com login válida e password inexistente. |

| **Passos**                                                                    |
| :---------------------------------------------------------------------------- |
| **DADO** que o usuário está na página de login (https://www.saucedemo.com/v1/index.html)     |
| **QUANDO** ele insere o username cadastrado e a senha incorreta                   |
| **E** clica no botão "login"                                                  |
| **ENTÃO** ele deve permanecer na página para a página inicial da aplicação (ou homepage) |
| **E** um erro deve ser visível na tela                                                 |

| **Critérios de aceitação**                                                                            |
| :---------------------------------------------------------------------------------------------------- |
| O sistema deve permanecer na página de login e um erro evidenciando que o usarnem e o login estão inválido |


| **Evidência:** | 
| :---------------------------------------------------------------------------------------------------- |
|![Login sem sucesso](https://github.com/vnadoti/manual-test-swaglabs/blob/main/evidencias/login-invalid.gif)|

___ 

### 🔐Logout de Usuário
| ID                     | Descrição                                                             |
| :--------------------- | :-------------------------------------------------------------------- |
| TC-003 | Verifique se um usuário conectado pode efetuar logout. |

| **Pré-condições**                            |
| :------------------------------------------- |
| Usuário logado na aplicação. |

| **Passos**                                                                    |
| :---------------------------------------------------------------------------- |
| **DADO** que o usuário está na logado na  aplicação     |
| **QUANDO** ele clica no menu de navegação                  |
| **E** clica no botão "logout"                                                  |
| **ENTÃO** ele deve ser desconectado e redirecionado para a página de Login   |

| **Critérios de aceitação**                                                                            |
| :---------------------------------------------------------------------------------------------------- |
| O usuário é desconectado e redirecionado para a página de login |


| **Evidência:** | 
| :---------------------------------------------------------------------------------------------------- |
|![Logout](https://github.com/vnadoti/manual-test-swaglabs/blob/main/evidencias/logout.gif)|

___ 

### 🛒Ordenar Podutos de Ordem Alfabética ( A a Z ) e (Z a A )
| ID                     | Descrição                                                             |
| :--------------------- | :-------------------------------------------------------------------- |
| TC-004 | Ordenação dos produtos por ordem Alfabética (A a Z ) e (Z a A) |

| **Pré-condições**                            |
| :------------------------------------------- |
| Usuário logado na aplicação. |

| **Passos**                                                                    |
| :---------------------------------------------------------------------------- |
| **DADO** que o usuário está na página inicial da aplicação     |
| **QUANDO** ele seleciona a opção "Name: A to Z"                 |
| **ENTÃO** os produtos são ordenados por ordem alfabética de A para Z | 
| **QUANDO** ele seleciona a opção "Name: Z to A"                 |
| **ENTÃO** os produtos são ordenados por ordem alfabética de Z para A | 

| **Critérios de aceitação**                                                                            |
| :---------------------------------------------------------------------------------------------------- |
| Produtos exibidos na ordem correta conforme seleção |


| **Evidência:** | 
| :---------------------------------------------------------------------------------------------------- |
|![az](https://github.com/vnadoti/manual-test-swaglabs/blob/main/evidencias/ordering.gif)|

___ 
### 🛒Ordenar Podutos produtos por preço
| ID                     | Descrição                                                             |
| :--------------------- | :-------------------------------------------------------------------- |
| TC-005 | Ordenação dos produtos por preço do menor para o maior e vice-versa |

| **Pré-condições**                            |
| :------------------------------------------- |
| Usuário logado na aplicação. |

| **Passos**                                                                    |
| :---------------------------------------------------------------------------- |
| **DADO** que o usuário está na página inicial da aplicação     |
| **QUANDO** ele seleciona a opção "Price: low to high”     |
| **ENTÃO** os produtos são ordenados do mais barato para o mais caro |
| **QUANDO** ele seleciona a opção "Price: high to low"     |
| **ENTÃO** os produtos são ordenados do mais caro para o mais barato | 

| **Critérios de aceitação**                                                                            |
| :---------------------------------------------------------------------------------------------------- |
| Produtos exibidos na ordem correta de preço conforme seleção |


| **Evidência:** | 
| :---------------------------------------------------------------------------------------------------- |
|![prices](https://github.com/vnadoti/manual-test-swaglabs/blob/main/evidencias/ordering.gif)|



### 🛒Adicionar Produtos ao carrinho
| ID                     | Descrição                                                             |
| :--------------------- | :-------------------------------------------------------------------- |
| TC-006 | Verifique se um usuário logado pode adicionar produtos no carrinho de compras  |

| **Pré-condições**                            |
| :------------------------------------------- |
| Usuário logado na aplicação. |

| **Passos**                                                                    |
| :---------------------------------------------------------------------------- |
| **DADO** que o usuário está na página inicial da aplicação     |
| **QUANDO** ele escolhe o produto que deseja adicionar                  |
| **E** clica no botão "Add to cart"                                                  |
| **ENTÃO** O produto é adicionado e exibido um número no icone de carrinho   |

| **Critérios de aceitação**                                                                            |
| :---------------------------------------------------------------------------------------------------- |
| É acrescentado no icone de carrinho |


| **Evidência:** | 
| :---------------------------------------------------------------------------------------------------- |
|![Add to Cart](https://github.com/vnadoti/manual-test-swaglabs/blob/main/evidencias/carrinho.gif)|

___ 

### 🛒Remover Produtos ao carrinho
| ID                     | Descrição                                                             |
| :--------------------- | :-------------------------------------------------------------------- |
| TC-007 | Verifique se um usuário logado pode remover produtos do carrinho de compras   |

| **Pré-condições**                            |
| :------------------------------------------- |
| Ter produtos adicionado no carrinho |

| **Passos**                                                                    |
| :---------------------------------------------------------------------------- |
| **DADO** que o usuário está na página inicial da aplicação     |
| **QUANDO** ele escolhe o produto que deseja remover                 |
| **E** clica no botão "Remove"                                                  |
| **ENTÃO** O produto é removido do carrinho e o icone é atualizado   |

| **Critérios de aceitação**                                                                            |
| :---------------------------------------------------------------------------------------------------- |
| É retirado o produto do carrinho e atualizado no icone de carrinho |


| **Evidência:** | 
| :---------------------------------------------------------------------------------------------------- |
|![Remove to Cart](https://github.com/vnadoti/manual-test-swaglabs/blob/main/evidencias/carrinho.gif)|

___ 

### 🛒Continuar Comprando
| ID                     | Descrição                                                             |
| :--------------------- | :-------------------------------------------------------------------- |
| TC-008 | O usuário clica em "Continuar Comprando" e é redirecionado adequadamente.    |

| **Pré-condições**                            |
| :------------------------------------------- |
| Usuário está na página do carrinho. |

| **Passos**                                                                    |
| :---------------------------------------------------------------------------- |
| **DADO** que o usuário está na página do carrinho |
| **QUANDO** ele clica no botão/link “Continue Shopping” |
| **ENTÃO** ele deve ser redirecionado para a homepage |

| **Critérios de aceitação**                                                                            |
| :---------------------------------------------------------------------------------------------------- |
| O sistema redireciona corretamente o usuário para continuar navegando. |


| **Evidência:** | 
| :---------------------------------------------------------------------------------------------------- |
|![Continue Shopping](https://github.com/vnadoti/manual-test-swaglabs/blob/main/evidencias/continue-shopping.gif)|

___ 

### 🛒Prosseguir para Checkout
| ID                     | Descrição                                                             |
| :--------------------- | :-------------------------------------------------------------------- |
| TC-009 | O usuário inicia o processo de checkout ao clicar no botão.    |

| **Pré-condições**                            |
| :------------------------------------------- |
| Itens presentes no carrinho. |

| **Passos**                                                                    |
| :---------------------------------------------------------------------------- |
| **DADO** que o usuário está na página do carrinho com itens |
| **QUANDO** ele clica no botão "Checkout" |
| **ENTÃO** ele deve ser redirecionado para a primeira etapa do processo de checkout |

| **Critérios de aceitação**                                                                            |
| :---------------------------------------------------------------------------------------------------- |
| O sistema inicia o processo de checkout redirecionando o usuário corretamente |


| **Evidência:** | 
| :---------------------------------------------------------------------------------------------------- |
|![Chekout](https://github.com/vnadoti/manual-test-swaglabs/blob/main/evidencias/checkout.gif)|

___ 

### 🛒Validação de Campos para Checkout
| ID                     | Descrição                                                             |
| :--------------------- | :-------------------------------------------------------------------- |
| TC-010 | Tentativa de avançar no checkout sem preencher campos obrigatórios.|

| **Pré-condições**                            |
| :------------------------------------------- |
| Iniciado a Etapa de Chekout |

| **Passos**                                                                    |
| :---------------------------------------------------------------------------- |
| **DADO** que o usuário logado está na etapa de "Your Information" do checkout|
| **QUANDO** ele tenta continuar sem preencher um ou mais campos obrigatórios (ex: Nome, CEP) |
| **ENTÃO** mensagens de erro devem ser exibidas para cada campo obrigatório não preenchido |
| **E** ele não deve avançar para a próxima etapa |

| **Critérios de aceitação**                                                                            |
| :---------------------------------------------------------------------------------------------------- |
| O sistema deve bloquear a navegação e mostrar mensagens de erro específicas. |


| **Evidência:** | 
| :---------------------------------------------------------------------------------------------------- |
|![Chekout fields](https://github.com/vnadoti/manual-test-swaglabs/blob/main/evidencias/checkout-fields.gif)|

___ 

### 🛒Revisão do Pedido antes da Finalização do Pagamento
| ID                     | Descrição                                                             |
| :--------------------- | :-------------------------------------------------------------------- |
| TC-011 | Usuário revisa o pedido antes de finalizar a compra.|

| **Pré-condições**                            |
| :------------------------------------------- |
| Usuário está na última etapa do checkout antes de finalizar.|

| **Passos**                                                                    |
| :---------------------------------------------------------------------------- |
| **DADO** que o usuário está na última etapa do checkout, antes de clicar em "Finish"|
| **ENTÃO** um resumo completo do pedido deve ser visível, incluindo: |
| - Quantidade e Descrição dos produtos | 
| - Informações do Método de Pagamento | 
| - Método de envio selecionado e custo |
| - Subtotal, impostos (se houver), frete e total geral| 

| **Critérios de aceitação**                                                                            |
| :---------------------------------------------------------------------------------------------------- |
| O sistema deve mostrar um resumo detalhado e correto do pedido antes da finalização. |


| **Evidência:** | 
| :---------------------------------------------------------------------------------------------------- |
|![Overview](https://github.com/vnadoti/manual-test-swaglabs/blob/main/evidencias/overview.png)|

___ 

### 🛒 Finalização do pedido
| ID                     | Descrição                                                             |
| :--------------------- | :-------------------------------------------------------------------- |
| TC-012 | Usuário finaliza o pedido na demo.|

| **Pré-condições**                            |
| :------------------------------------------- |
| Usuário revisado o carrinho de compra|
	
| **Passos**                                                                    |
| :---------------------------------------------------------------------------- |
| **DADO** que o usuário está na última etapa do checkout|
| **QUANDO** clicar em “Finish” | 
| **ENTÃO** O sistema deverá processar o pedido |
| **E** redirecionar para uma página de “Thank You”|

| **Critérios de aceitação**                                                                            |
| :---------------------------------------------------------------------------------------------------- |
| O sistema deve processar o pedido e redirecionar para a página de Thank You. |


| **Evidência:** | 
| :---------------------------------------------------------------------------------------------------- |
|![Thank You](https://github.com/vnadoti/manual-test-swaglabs/blob/main/evidencias/thank-you.png)|
