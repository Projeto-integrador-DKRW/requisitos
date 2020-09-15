# requisitos

Requisitos Funcionais do projeto


01.1- Tela inicial – Terá duas opções de acesso para o aplicativo, podendo o usuário selecionar se o mesmo entrará como responsável do restaurante, ou como cliente.

02.1– Área do Restaurante - Será obrigatório o cadastro do restaurante, e o mesmo será realizado pelo responsável da franquia (Gerente e etc.).

03.1 – Tela de Cadastro do Restaurante – Será solicitado o CNPJ do restaurante, e ao preencher o campo de CNPJ será feita uma requisição para a API da receita federal de consulta de CNPJ, para verificar a situação do restaurante. Após isso, será solicitado informar a sede onde será utilizado o app. Os dados pessoais do responsável pelo restaurante (gerente e afins), serão informados e enviados para o e-mail que a API da receita devolve no formato JSON, referente ao Sócio da empresa, para realizar a confirmação que a pessoa que está cadastrando o restaurante, realmente trabalha lá. Ao autorizar, será redirecionado a uma página de confirmação.

03.2 – Menu Principal Restaurante – No menu principal, terá 4(quatro) Sub-Menus denominados ‘Informações ’, ‘Cardápio’, ‘Promoções’ e ‘Pedidos’ e cada um levará para sua respectiva tela.

04.1 – Tela de Informações – Nesta tela serão adicionadas informações sobre a loja, como os Horários de funcionamento e os dados para contato. (Obrigatório)

04.2 – Tela do Cardápio – Nesta tela, serão adicionados/alterados os itens do cardápio. (Obrigatório).

04.3 – Tela de Promoções – Nesta tela será permitido adicionar as promoções (Opcional).

04.4 – Tela de Pedidos – Nesta tela terá 3 (três) opções, ‘Pedidos realizados’, ‘Anotar Pedidos’ e ‘Finalizar Mesa’. Ao selecionar a opção Pedidos realizados, poderá ser consultado todos os pedidos já feitos, e atualizar os status de cada um como ‘pendente’, ‘fazendo’, ‘pronto’ e ‘entregue’.
Ao acessar a tela ‘Anotar pedidos’, será realizado a anotação apenas dos pedidos dos clientes que estão no restaurante, e ao final do pedido será informado a mesa onde o cliente se encontra, e gerará um código QR para que o cliente possa acompanhar o seu pedido. O valor do pedido será guardado, no app. E poderá ser consultado no menu ‘Finalizar Mesa’ que também servirá como controle na hora de pedir as contas.

Na tela finalizar mesa, terá um Grid contendo todas as mesas e seus status ao lado como ‘pedidos realizados’, ‘pedidos entregues’, e ‘finalização de conta’

Caso o status da mesa esteja ‘finalização de conta’, o funcionário deverá ir a mesa para processar a solicitação de finalização, e para maior organização, o funcionário deve informar o seu nome e atualizar o status par’, para indicar que ele está indo atender a solicitação da mesa em questão, para que vários funcionários não vão para a mesma mesa.


05.1 – Área do cliente   - Ao entrar na área do cliente, serão apresentadas 3 (três) opções 'Login' , 'Cadastre-se' e 'Prosseguir sem Login'

06.1 - Tela de Login - Ao entrar na tela de Login, será apresentados os campos de email e senha para logar, assim como o link 'Esqueci minha senha' caso o cliente tenha esquecido sua senha.
 Ao clicar no Link 'Esqueci minha senha', será enviado um email para o cliente, para que ele possa alterar a mesma.

07.1 - Tela 'Cadastre-se' - Ao entrar nesta tela, serão apresentados  os campos de preenchimento obrigatorio referente aos dados pessoais do cliente (Nome, CPF, email, senha, celular).

08.1 - Tela Prosseguir sem Login - Ao escolher esta opção, o usuário será redirecionado diretamente ao menu principal do cliente.

09.1 – Menu principal do cliente - Ao entrar no menu do cliente, serão apresentados 3(três) Sub-Menus denominados ‘Realizar Pedido’, ‘Consultar Pedido’ e ‘Pedir a conta’

10.1 – Tela Realizar Pedido – Esta tela será a responsável pelo cliente escolher os itens que ele deseja pedir. Ao término do Pedido, será apresentado uma mensagem perguntando se o cliente está em uma mesa do restaurante, caso a resposta for sim, deverá ser informado a mesa onde ele se encontra, e ao final, gerará o código do pedido, e uma mensagem, perguntando se o mesmo quer que seja direcionado a página de consulta de pedidos.

10.2 – Tela Consultar pedido – Nesta tela o cliente poderá consultar o seu pedido, caso o pedido tenha sido feito pelo próprio cliente, ele poderá consultar o pedido pelo código gerado no aplicativo para ele, ou caso o pedido seja feito por um dos funcionários da loja, o cliente terá a opção de consultar o pedido pelo código QR gerado no aparelho do funcionário.

10.3 – Tela Pedir a conta – Nesta tela o cliente poderá consultar o valor dos seus pedidos, pelo Número da mesa, assim como no item 04.4, e terá a opção de fechar a conta da mesa.
Ele terá duas opções, pagar pelo aplicativo, ou chamar o funcionário para realizar o pagamento.
Independente da escolha a cima, será enviado a solicitação para o restaurante, e solicitação ficará salva na tela ‘Finalizar Mesa’ na área do restaurante, destacada em vermelho, mudando apenas o status de pago.


Requisitos não funcionais do Projeto

01.1 – Desempenho – O app deve ser rápido em suas transições e rápido em suas consultas no banco.

02.1 – Usabilidade – O app deve ter uma interface muito simples e intuitiva para que os usuários, sendo gerentes ou clientes, não fiquem com dúvidas onde clicar.

03.1 – Testes – Na fase de desenvolvimento deverá ser realizados testes unitários afim de entregar para o cliente uma melhor experiencia sem obstáculos.

04.1 – Segurança – O app deverá ter segurança como token de autenticação para fazer requests nas APIs internas, exemplo JWT para alteração.

05.1 – Disponibilidade – O app estará disponível nas lojas dos celulares Android e IOS.

06.1 – Compatibilidade – O app estará disponível para as versões mais atuais de cada sistema operacional e para grande parte das antigas.
 
07.1 – Histórico  - O app salvará dados em tabelas de log especificas no banco, para captar alterações e verificações de rendimento do aplicativo.

08.1 – Servidor  – O banco de dados e as APIs estarão hospedadas em um servidor Linux onde será mais estável

09.1 - Design - O aplicativo deverá ter um design inovador, mas sem exageros, para que chame a atenção do cliente na hora de utiliza-lo.

10.1 - Manutenibilidade - O aplicativo deverá ser aberto a melhorias e reparos, de uma forma em que não prejudique o cliente e a sua usabilidade.

