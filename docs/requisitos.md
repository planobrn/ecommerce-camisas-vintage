### Processo de eng. de software

O processo adotado para o desenvolvimento desse e-commerce é o Iterativo e Incremental, pois possibilita a entrega do produto em incrementos, adicionando funcionalidades ao longo do desenvolvimento e gerando valor para o cliente. Além disso, permite que mudanças nos requisitos sejam realizadas durante o processo, possibilitando a aplicação de melhorias e inclusão de novas funcionalidades, através de revisões e feedback do cliente. Esse processo é adequado ao projeto, pois suas diversas funcionalidades podem ser desenvolvidas e avaliadas gradualmente, permitindo que o sistema seja aprimorado conforme as necessidades identificadas. 

### Requisitos Funcionais

1. RF1 → Cadastro de clientes    
    Descrição: O sistema deve permitir que o cliente realize seu cadastro utilizando e-mail ou número de celular e senha, enviando um código de confirmação para validar o cadastro.
    
2. RF2 → Login    
    Descrição: O sistema deve permitir que o cliente realize login para acessar os serviços do sistema e efetuar a compra de produtos.
    
3. RF3 → Cadastro de produtos    
    Descrição: O administrador deve conseguir cadastrar e alterar as informações dos produtos, incluindo a quantidade disponível em estoque.
    
4. RF4 → Filtros de produtos    
    Descrição: O sistema deve permitir que o cliente filtre os produtos por características como tipo de roupa, time, ano do uniforme, tamanho e gênero.
    
5. RF5 → Pesquisa de produtos    
    Descrição: O cliente deve ter a opção de buscar por um produto específico através de uma barra de pesquisa.
    
6. RF6 → Carrinho de compras     
    Descrição: O sistema deve permitir que o cliente adicione produtos ao carrinho de compras e posteriormente efetue a compra.
    
7. RF7 → Finalização do pedido    
    Descrição: O sistema deve permitir que o cliente revise os produtos selecionados no carrinho de compras, informe os dados necessários para a entrega e confirme o pedido antes de realizar o pagamento.
    
8. RF8 → Pagamentos com cartões    
    Descrição: O sistema deve permitir o pagamento por cartões de crédito e débito das bandeiras Visa, Mastercard e Elo.
    
9. RF9→ Pagamentos via Pix    
    Descrição: O sistema deve permitir o pagamento via Pix por meio de um QR Code ou Pix Copia e Cola.
    
10. RF10→ Emissão de nota fiscal    
    Descrição: O sistema deve emitir nota fiscal após a compra e enviar por e-mail para o cliente.
    

### Requisitos não Funcionais

1. RNF1 → Quantidade de usuários simultâneos (Desempenho)    
    Descrição:  O sistema ser construído para ter capacidade de acesso simultâneo de até 5.000 clientes.
    
2. RNF2 → Tempo máximo de resposta (Desempenho)    
    Descrição:  O sistema deve apresentar resposta de até 2 segundos após uma ação realizada pelo usuário ou administrador.
    
3. RNF3 → Emissão de nota fiscal (Desempenho)    
    Descrição:  O sistema deve emitir a nota fiscal em até 5 minutos após a confirmação do pagamento.
    
4. RNF4 →  Restrição de acesso (Segurança)    
    Descrição:  O sistema não deve permitir o acesso quando o e-mail, número de telefone ou a senha forem inválidos, apresentando uma mensagem de erro ao usuário.
    
5. RNF5 → Proteção de senhas (Segurança)    
    Descrição:   O sistema deve armazenar as senhas dos usuários de maneira segura, não permitindo que sejam armazenadas ou visualizadas em formato aberto.
    
6. RNF7 → Compatibilidade Web (Ambiente)    
    Descrição:   O sistema deve funcionar em ambiente Web, sendo compatível com os principais navegadores atuais: Chrome, Safari, Opera e Edge.
    
7. RNF6 → Compatibilidade Mobile (Ambiente)    
    Descrição:  O sistema deve funcionar em dispositivos móveis com sistemas Android e iOS, apresentando uma interface adaptada para esses dispositivos.
    
8. RNF8 → Front-end (Linguagem)    
    Descrição:  O sistema deve ser desenvolvido utilizando JavaScript juntamente com React para o Front-end.
    
9. RNF9 → Back-end (Linguagem)     
    Descrição:  O sistema deve ser desenvolvido utilizando Python e o framework FastAPI para o Back-end.
    
10. RNF10→ Banco de dados (Tecnologia)
    Descrição:  O PostgreSQL deverá ser utilizado para armazenar as informações do sistema, como usuários, produtos, estoque e pedidos.
    

### User Stories

1. RF1 → Cadastro de clientes
    
    User story: Como cliente, quero realizar o cadastro com meus dados para ter acesso ao sistema.
    
    Critérios de aceitação:    
    - O sistema deve permitir que o cliente realize o cadastro utilizando e-mail ou número de celular e senha.
    - O sistema deve verificar os dados através de um código de validação enviado por e-mail.
    - O cadastro deve ser concluído somente após a confirmação do código enviado.
      
2. RF2 → Login
    
    User stories: Como cliente, quero fazer login no sistema para poder escolher os produtos e fazer a compra. 
    
    Critérios de aceitação:
    - O sistema deve permitir que o cliente realize o login através de e-mail ou número de celular e senha cadastrados.
    - O sistema deve validar os dados preenchidos e liberar o acesso caso estejam corretos.
    - Caso os dados estejam incorretos, o sistema deve apresentar uma mensagem de erro.
      
3. RF3 → Cadastro de produtos
    
    User stories: Como administrador, quero cadastrar os produtos no sistema para poder disponibilizá-los para os clientes.
    
    Critérios de aceitação:
    - O sistema deve permitir que o administrador cadastre novos produtos.
    - O sistema deve permitir que o administrador informe a quantidade de produtos disponíveis em estoque.
    - O sistema deve permitir que o administrador altere as informações dos produtos cadastrados.
      
4. RF4 → Filtros de produtos
    
    User stories: Como cliente, quero aplicar filtros aos produtos para encontrar produtos de acordo com minhas preferências.
    
    Critérios de aceitação:    
    - O sistema deve permitir que o cliente selecione os filtros desejados.
    - O sistema deve disponibilizar filtros sobre as características dos produtos.
    - O sistema deve apresentar uma mensagem caso não haja produtos com os filtros selecionados.
      
5. RF5 → Pesquisa de produtos
    
    User stories: Como cliente, quero fazer pesquisas diretas para conseguir achar um determinado produto com facilidade.
    
    Critérios de aceitação:    
    - O sistema deve permitir que o cliente busque por produtos conforme a pesquisa.
    - O sistema deve apresentar após a busca, somente produtos relacionados à pesquisa.
    - O sistema deve apresentar uma mensagem caso não haja produtos relacionados à pesquisa.
      
6. RF6 → Carrinho de compras
    
    User stories: Como cliente, quero adicionar produtos ao carrinho de compras para visualizar os produtos escolhidos.
    
    Critérios de aceitação:
    - O sistema deve adicionar ao carrinho de compras os produtos selecionados pelo cliente.
    - O sistema deve apresentar no carrinho de compras a quantidade de produtos que o cliente selecionou.
    - O sistema deve calcular o valor total dos produtos selecionados pelo cliente.
      
8. RF7 → Finalização de compra
    
    User stories: Como cliente, quero revisar os produtos escolhidos e inserir meus dados para entrega para que eu confirme meu pedido.
    
    Critérios de aceitação    
    - O sistema deve apresentar os produtos selecionados e o valor total do pedido.
    - O sistema deve solicitar os dados do cliente para entrega dos produtos.
    - O sistema deve permitir que o cliente confirme o pedido antes de realizar o pagamento.
      
9. RF8 → Pagamento com Cartões
    
    User stories: Como cliente, quero usar meu cartão de crédito ou débito para finalizar minha compra.
    
    Critérios de aceitação
    - O sistema deve permitir o pagamento com cartões de crédito e débito.
    - O sistema deve verificar se o cartão pertence às bandeiras Visa, Mastercard ou Elo.
    - O sistema deve processar o pagamento caso os dados do cartão estejam válidos.
      
10. RF9 → Pagamento via Pix
    
    User stories: Como cliente, quero efetuar o pagamento por Pix para finalizar minha compra.
    
    Critérios de aceitação:    
    - O sistema deve disponibilizar a opção de pagamento via Pix.
    - O sistema deve disponibilizar um QR Code ou Pix Copia e Cola para que o cliente faça o pagamento.
    - O sistema deve confirmar o pagamento após a realização da transação.
      
11. RF10 → Emissão de nota fiscal
    
    User stories: Como cliente, quero receber a nota fiscal da minha compra para ter a comprovação da compra realizada.
    
    Critérios de aceitação:    
    - O sistema deve emitir a nota fiscal após a confirmação do pagamento.
    - O sistema deve enviar a nota fiscal para o e-mail cadastrado pelo cliente.
    - A nota fiscal deve corresponder ao pedido realizado pelo cliente.
