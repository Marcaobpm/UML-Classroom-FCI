<h2><a href= "https://www.mackenzie.br">Universidade Presbiteriana Mackenzie</a></h2>
<h3><a href= "https://www.mackenzie.br/graduacao/sao-paulo-higienopolis/sistemas-de-informacao">Sistemas de Informação</a></h3>


<font size="+22"><center>
Solução Pizzaria Express
</center></font>


# Autores

* Marcos Antonio
* Pedro Araujo


# Descrição do Projeto

A Pizza-Express, uma rede de fast-food com 40 lojas, enfrentou uma queda de 30% em suas vendas devido a um serviço de entrega lento, que prometia uma hora, em contraste com seu concorrente que entregava em 30 minutos. Para reverter essa situação, o gerente de sistemas de informação, Marcos e Pedro, foram encarregados de desenvolver um novo sistema de software.

O projeto tem dois focos principais:

Sistema de Atendimento de Pedidos: Identificar a loja mais próxima do cliente para otimizar o tempo de entrega.
Sistema de Operação de Fábricas de Pizzas: Criar unidades de entrega dedicadas, sem espaço de varejo, que garantam a entrega em 10 a 15 minutos.
Com o apoio da Papa-Léguas Delivery, a equipe deve implementar soluções tecnológicas e logísticas eficientes para aumentar a competitividade da Pizza-Express no setor de delivery.

# Análise de Requisitos Funcionais e Não-Funcionais

Análise de Requisitos
Problema: A Pizza-Express tem perdido 30% do seu faturamento por não conseguir competir com a concorrência, que promete entregas em 30 minutos. A Pizza-Express atualmente anuncia entrega em uma hora e não possui um sistema eficaz para processar as entregas de forma rápida. A empresa precisa de um sistema que reduza o tempo de entrega para menos de 30 minutos, garantindo competitividade e eficiência no serviço de delivery.
Objetivo: Desenvolver dois sistemas de software que permitam à Pizza-Express competir com seus concorrentes, garantindo entregas rápidas e eficientes:

Sistema de Atendimento de Pedidos: Identificar a loja mais próxima do cliente e encaminhar o pedido para ela.
Sistema de Operações da Fábrica de Pizzas: Gerenciar a produção e entrega das pizzas de forma otimizada para garantir o atendimento em até 15 minutos desde a entrada do pedido até a saída para entrega. 
Requisitos Funcionais:
Localização Automática da Loja: Identificar a loja mais próxima do cliente para agilizar o processo.
Gestão de Pedidos: Processar e distribuir pedidos para as lojas mais próximas, com personalização.
Estimativa de Tempo de Entrega: Calcular e informar o tempo estimado ao cliente.
Rastreamento em Tempo Real: Oferecer rastreamento do pedido até a entrega.
Gestão de Estoque e Preparo: Verificar estoque, iniciar preparo e garantir tempo máximo de preparo de 10 a 15 minutos.
Notificações ao Cliente: Enviar atualizações sobre o status do pedido.
Integração com Serviços de Entrega: Integrar com sistemas de entrega terceirizados, se necessário.
Requisitos Não Funcionais:
Desempenho: Suportar até 1000 pedidos simultâneos por loja.
Segurança: Proteger dados sensíveis dos clientes.
Escalabilidade: Permitir crescimento no número de lojas e pedidos.
Usabilidade: Interface simples para facilitar o uso pelos funcionários.
Disponibilidade: Garantir 99,9% de disponibilidade. 

# Diagrama de Atividades

*&lt;
![Classe UML](https://github.com/user-attachments/assets/59b30010-3fd1-46b5-9621-cdd87c4a430b)


&gt;*

# Diagrama de Casos de Uso

![Diagrama de Casos de uso-1](https://github.com/user-attachments/assets/e95dbdfd-a677-427b-bc78-a75247e006b3)


# Descrição dos Casos de Uso

Caso 1  

Fazer Pedido 

 Ator Principal - Cliente  

  

Objetivo - Permitir que o cliente faça um pedido de pizza  

  

Pré-condições - O cliente deve ter acesso ao aplicativo ou site  

  

Fluxo Principal -  

 O cliente acessa o aplicativo/site.  

 O cliente seleciona a opção de fazer um pedido.  

 O sistema localiza a loja mais próxima.  

 O cliente escolhe itens do menu.  

 O cliente confirma o pedido.  

 

Fluxos Alternativos - Se a loja não estiver disponível, o sistema sugere outra loja 

 

Caso 2  

 Localizar Loja  

 Ator Principal - Sistema  

  

Objetivo - Identificar a loja mais próxima do cliente  

  

Pré-condições - O cliente deve permitir acesso à localização  

  

Fluxo Principal  

 O sistema solicita a localização do cliente.  

 O sistema identifica a loja mais próxima com base na localização.  

  

 Fluxos Alternativos - Se a localização não puder ser determinada, o sistema pede que o cliente insira o endereço manualmente 

Caso 3  

 Exibir Menu  

  

Ator Principal - Sistema  

  

Objetivo - Mostrar o menu da loja selecionada  

  

Pré-condições - A loja mais próxima deve ter sido identificada  

  

Fluxo Principal  

 O sistema exibe o menu da loja mais próxima  

  

Fluxos Alternativos - Se a loja não tiver itens disponíveis, o sistema notifica o cliente 

 

 

Confirmar Pedido  

  

 Ator Principal - Cliente  

  

Objetivo - Confirmar os itens selecionados e finalizar o pedido  

  

Pré-condições - O cliente deve ter selecionado itens do menu  

  

Fluxo Principal  

 O cliente revisa o pedido.  

 O cliente confirma o pedido.  

 O sistema processa o pedido.  

  

Fluxos Alternativos - O cliente pode cancelar o pedido antes de confirmar 

Calcular tempo de espera  

  

 Ator Principal - Sistema  

  

Objetivo - Informar o cliente sobre o tempo estimado de entrega  

  

Pré-condições - O pedido deve estar confirmado.  

  

Fluxo Principal - 

 O sistema calcula o tempo estimado de entrega.  

 O sistema informa o cliente sobre o tempo estimado.  

  

Fluxos Alternativos - Se houver atrasos, o sistema notifica o cliente  

 

 

 

Caso 6  

 Gerenciar Pedidos  

  

 Ator Principal - Funcionário da loja  

  

Objetivo - Gerenciar os pedidos recebidos na loja  

  

Pré-condições - O pedido deve estar registrado no sistema  

  

Fluxo Principal - 

 O funcionário acessa a lista de pedidos.  

 O funcionário visualiza os detalhes do pedido.  

 O funcionário atualiza o status do pedido.  

  

Fluxos Alternativos - Se o pedido não puder ser processado, o funcionário notifica o cliente 

 

 

Caso 7  

Verificar estoque  

  

 Ator Principal - Sistema  

  

Objetivo - Garantir que os itens do pedido estão disponíveis  

  

Pré-condições - Um pedido deve estar em processo  

  

Fluxo Principal  

 O sistema verifica a disponibilidade dos itens.  

 O sistema atualiza o status do estoque  

  

Fluxos Alternativos - Se um item não estiver disponível, o sistema notifica o funcionário 

 

 

 

 

 

Caso 8  

 Preparar Pedido  

  

 Ator Principal - Funcionário da Loja  

  

Objetivo - Preparar o pedido conforme solicitado pelo cliente.  

  

Pré-condições - O pedido deve ter sido confirmado  

  

Fluxo Principal  

 O funcionário inicia a preparação do pedido.  

 O funcionário registra o tempo de preparo.  

 O funcionário finaliza o pedido.  

  

Fluxos Alternativos - Se houver problemas na preparação, o funcionário notifica o cliente 

 

 

 

 

Caso 9  

 Notificar Cliente  

  

Ator Principal - Sistema  

  

Objetivo - Informar o cliente sobre o status do pedido  

  

Pré-condições - Um pedido deve estar em processamento  

  

Fluxo Principal  

 O sistema envia notificações ao cliente sobre atualizações do pedido  

  

Fluxos Alternativos - Se a entrega for atrasada, o sistema notifica o cliente imediatamente 

 

Caso 10  

Rastrear Pedido  

  

Ator Principal - Cliente  

  

Objetivo - Permitir que o cliente acompanhe seu pedido em tempo real  

  

Pré-condições - O pedido deve estar em processo de entrega  

  

Fluxo Principal  

O cliente acessa a função de rastreamento.  

O sistema exibe a localização do entregador e o status do pedido.  

  

Fluxos Alternativos - Se o sistema não puder acessar a localização, informa que está indisponível 

 

 

 

 

 

Caso 11  

Realizar Entrega  

  

Ator Principal - Sistema de Entrega  

  

Objetivo - Garantir que o pedido seja entregue ao cliente  

  

Pré-condições - O pedido deve estar pronto para entrega  

  

Fluxo Principal  

 O sistema de entrega coleta o pedido na loja.  

 O entregador leva o pedido até o cliente.  

  

Fluxos Alternativos - Se houver problemas de entrega, o sistema notifica o cliente e a loja  

  

 

 

 

 

Caso 12  

Gerenciar as Configurações do sistema  

  

Ator Principal - Administrador  

  

Objetivo - Permitir que o administrador gerencie o sistema  

  

Pré-condições - O administrador deve estar autenticado  

  

Fluxo Principal  

O administrador acessa o painel de controle.  

O administrador modifica as configurações do sistema.  

O administrador salva as alterações.  

  

Fluxos Alternativos - Se as alterações não puderem ser salvas, o sistema exibe um erro




# Referências

      Pressman, R. S., & Maxim, B. R. (2021). Engenharia de software (9th ed.). 

      Link da URL:  https://app.minhabiblioteca.com.br/books/9786558040118

          Filho, W.D.P. P. (2019). Engenharia de Software – Produtos – Vol.1 (4th ed.).

            Link da URL:  https://app.minhabiblioteca.com.br/books/9788521636724

                Pressman, R. S., & Maxim, B. R. (2021). Engenharia de software (9th ed.). 

                Link da URL:  https://app.minhabiblioteca.com.br/books/9786558040118

              Pressman, R. S., & Maxim, B. R. (2021). Engenharia de software (9th ed.). 

                Link da URL:  https://app.minhabiblioteca.com.br/books/9786558040118

      Pressman, R. S., & Maxim, B. R. (2021). Engenharia de software (9th ed.). 

                Link da URL: https://app.minhabiblioteca.com.br/books/9786558040118

                Filho, W.D.P. P. (2019). Engenharia de Software – Produtos – Vol.1 (4th ed.).

            Link da URL:  https://app.minhabiblioteca.com.br/books/9788521636724

