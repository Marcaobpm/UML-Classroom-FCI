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





# Diagrama de Sequência
[Diagrama de Sequencia.pdf](https://github.com/user-attachments/files/17950194/Diagrama.de.Sequencia.pdf)
Esse diagrama é um diagrama de sequência, usado para representar o fluxo de interação entre diferentes atores e sistemas ao longo do tempo. Ele é muito comum em engenharia de software e projetos de sistemas. Vamos analisá-lo:

Componentes do diagrama:
Atores e sistemas (colunas):

Cliente: O usuário que inicia o processo.
Sistema: O sistema responsável por processar o pedido.
Loja: Local onde a pizza será preparada.
Cozinha: A área que efetivamente prepara a pizza.
Entregador: Responsável por entregar o pedido ao cliente.
Mensagens (setas):

As setas representam as interações entre os elementos (atores ou sistemas) e são organizadas cronologicamente, de cima para baixo.
Lifelines (linhas verticais):

Representam a existência dos atores ou sistemas ao longo do processo.
Explicação do fluxo:
Início do pedido:

O cliente inicia o pedido enviando uma solicitação ao Sistema.
Identificar loja próxima:

O sistema verifica qual loja está mais próxima e envia uma mensagem de identificação.
A loja responde confirmando que foi identificada.
Preparar pizza:

O sistema solicita à loja que prepare a pizza, e a loja, por sua vez, repassa a tarefa à cozinha.
A cozinha prepara a pizza e notifica a loja quando estiver pronta.
Cálculo do tempo de entrega:

O sistema calcula o tempo estimado de entrega com base na localização e status do pedido.
Envio para entrega:

A loja solicita ao entregador que faça a entrega da pizza ao cliente.
Finalização do pedido:

O sistema finaliza o pedido e encerra o processo.
Finalidade do diagrama:
Ele ajuda a:

Compreender o fluxo de comunicação entre os elementos.
Visualizar a sequência lógica das interações.
Identificar possíveis falhas ou gargalos no processo.






# Diagrama de Classes
[Blank diagram (2).pdf](https://github.com/user-attachments/files/17950209/Blank.diagram.2.pdf)

Elementos do diagrama:
Classes (retângulos com três divisões):

Cada classe é representada por um retângulo dividido em três partes:
O nome da classe (ex.: GerenciarConfigurações).
Atributos (não mostrados aqui, mas estariam abaixo do nome da classe).
Métodos ou operações (ex.: +verificarEstoque(), +atualizarConfiguracoes()).
As classes principais no diagrama são:

Administrador: Classe associada a ações administrativas do sistema.
GerenciarConfigurações: Responsável por ações como verificarEstoque() e atualizarConfiguracoes().
Sistema: Classe central que gerencia pedidos e funcionalidades gerais.
GerenciarPedidos: Inclui métodos como verificarEstoque() e prepararPedido().
Cliente: Representa o usuário do sistema.
FazerPedido: Oferece funcionalidades relacionadas ao fluxo do pedido, como localizarLoja(), exibirMenu(), etc.
Relações entre as classes:

Associações:
Setas como "uses" ou "includes" indicam que uma classe depende ou colabora com outra.
Exemplo: A classe Administrador usa a classe GerenciarConfigurações.
Dependência ("includes"):
A classe GerenciarPedidos inclui funcionalidades da classe FazerPedido.
Direcionalidade:
As setas mostram o fluxo de dependência entre as classes.
Métodos:

Listados após o símbolo + (indica que são públicos). Cada método representa uma ação ou operação oferecida pela classe.
Explicação do fluxo:
O Administrador usa a classe GerenciarConfigurações para tarefas administrativas, como verificar estoque e atualizar configurações.
O Sistema inclui a classe GerenciarPedidos, que organiza o preparo e o fluxo de pedidos.
O Cliente interage com o Sistema para realizar um pedido, utilizando a classe FazerPedido, que engloba operações como localizar loja, exibir menu e rastrear pedido.
Finalidade do diagrama:
Modelar a estrutura do sistema de forma orientada a objetos.
Definir as responsabilidades de cada classe e como elas se relacionam.
Servir como base para a implementação de código em linguagens orientadas a objetos, como Java, C#, etc.

# Diagrama de Estados
![Diagrama de estados](https://github.com/user-attachments/assets/99040c2c-fac7-4e53-8933-64dfbd3deb32)

Este diagrama de estados descreve o ciclo de vida de um pedido em um sistema, detalhando os estados e as transições entre eles. Abaixo, uma análise do processo representado:

Componentes do Diagrama
Estado Inicial e Final:

Estado Inicial: Representado pelo círculo preto no topo do diagrama. Marca o início do ciclo de vida do pedido.
Estado Final: Representado pelo círculo preto com borda dupla no final, indicando o término do processo.
Estados:

Início: Estado inicial do pedido.
RecebendoPedido: O sistema está processando o pedido inicial do cliente.
IdentificandoLoja: Determina qual loja será responsável pelo pedido.
PreparandoPedido: Momento em que a loja está produzindo o pedido (por exemplo, preparando uma pizza).
CalculandoEntrega: Estado em que o sistema calcula o tempo estimado para a entrega.
EnviandoEntrega: O pedido foi preparado e está sendo enviado para o cliente.
Finalizado: O pedido foi concluído e o ciclo está completo.
Transições:

As transições entre os estados são acionadas por eventos ou condições específicas, indicados pelos textos ao lado das setas:
"Pedido iniciado" → Transição do estado Início para RecebendoPedido.
"Pedido recebido" → Transição de RecebendoPedido para IdentificandoLoja.
"Loja identificada" → Transição de IdentificandoLoja para PreparandoPedido.
"Pizza preparada" → Transição de PreparandoPedido para CalculandoEntrega.
"Tempo de entrega calculado" → Transição de CalculandoEntrega para EnviandoEntrega.
"Pedido enviado para entrega" → Transição de EnviandoEntrega para Finalizado.
Fluxo Representado
O cliente inicia o processo, ativando o estado Início.
O pedido é recebido pelo sistema (RecebendoPedido).
O sistema identifica a loja mais próxima ou adequada para preparar o pedido (IdentificandoLoja).
A loja prepara o pedido (PreparandoPedido).
Após o preparo, o sistema calcula o tempo de entrega (CalculandoEntrega).
O pedido é enviado para entrega ao cliente (EnviandoEntrega).
O ciclo termina com o pedido finalizado (Finalizado).
Aplicações e Importância
Documentação: Este diagrama ajuda na documentação dos processos de negócio ou sistema.
Modelagem de Sistemas: É usado para planejar e compreender o comportamento do sistema em diferentes estados.
Melhoria de Processos: Ajuda a identificar gargalos ou pontos de melhoria no fluxo.
# Diagrama de Implantação
[Blank diagram (1) (1).pdf](https://github.com/user-attachments/files/17950249/Blank.diagram.1.1.pdf)

O diagrama apresentado é um diagrama de implementação, usado para ilustrar a arquitetura física de um sistema, mostrando como seus componentes de software e hardware estão conectados e interagem. Vamos analisá-lo em detalhes:

Estrutura do Diagrama
Elementos principais:
Cliente:
Representado pelo componente "Aplicativo Cliente". Este é o software que o usuário utiliza para acessar o sistema, provavelmente por meio de uma interface web ou aplicação específica.
Internet:
Indica que a comunicação entre o cliente e o sistema ocorre via conexão HTTP/HTTPS, sugerindo um sistema baseado na web.
Servidor Web:
Representa a camada responsável por processar as solicitações do cliente. É onde os serviços principais são executados, incluindo lógica de negócios.
Servidor de Banco de Dados:
Representado pelo "Banco de Dados", que armazena informações persistentes, como dados de clientes, pedidos ou configurações.
Serviço Web:
Inclui componentes como o "Frontend Web" e a "API REST", indicando que o sistema pode expor APIs para comunicação com outros serviços ou aplicações externas.
Relações e Conexões
Fluxo Cliente → Internet → Servidor Web:

O cliente se conecta ao servidor web através de protocolos HTTP/HTTPS, o que é típico em arquiteturas baseadas em REST ou aplicações web.
Servidor Web → Banco de Dados:

O servidor web se comunica com o banco de dados para consultas e atualizações. Essa conexão é essencial para persistir e recuperar dados necessários para a aplicação.
Serviço Web:

É indicado que o servidor web contém uma interface frontend e uma API REST. Essa arquitetura permite:
O acesso direto via navegador (frontend).
Integrações com outros sistemas ou serviços por meio da API REST.
Possíveis Interpretações
Este diagrama provavelmente descreve um sistema baseado na arquitetura cliente-servidor com foco em:
Conexões seguras (uso de HTTPS).
Separaçãode responsabilidades:
Cliente para interface de usuário.
Servidor web para lógica de negócios.
Banco de dados para persistência de dados.
Expansibilidade: A inclusão de uma API REST sugere que o sistema pode ser integrado a outras aplicações ou microserviços.
Benefícios do Diagrama
Clareza: Apresenta as camadas principais de interação entre cliente, servidor e banco de dados.
Escalabilidade: A presença de componentes como a API REST e o frontend indica que o sistema pode ser adaptado para diferentes plataformas ou dispositivos.
Segurança: A menção explícita de HTTPS sugere uma preocupação com a segurança das comunicações.




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

