# Projeto_Supera_front_React
 
# Como executar o aplicativo
 - Para executar o aplicativo, verifique se você tem o Node.js e o npm (Node Package Manager) instalados em sua máquina. Em seguida, siga estes passos:

- Abra um terminal ou prompt de comando.
- Navegue até o diretório do projeto.
- Instale as dependências necessárias executando o comando: npm install.
- Inicie o aplicativo executando o comando: npm start.
- O aplicativo agora deve estar em execução e acessível em http://localhost:3000.
 # Como funciona o componente
- O componente Table é um componente funcional que usa ganchos React, como useState e useEffect, para gerenciar o estado e executar efeitos colaterais.
- O componente importa vários componentes estilizados e um módulo api para fazer solicitações HTTP para um servidor back-end.
- O componente inicializa variáveis de estado usando o gancho useState, como transferencia (dados de transferência), total (número total de itens), limit (número de itens por página), pages (total de páginas) e currentPage (página atual).
- O componente também inicializa variáveis de estado para filtrar dados de transferência, como init (data inicial), end (data de término) e nomeOperador do operador).
- O componente usa o gancho useEffect para buscar dados de transferencia da API de back-end quando o componente é montado ou quando as variáveis currentPage, limit ou total state mudam.
- A função handleSubmitted é uma função de retorno de chamada que é acionada quando o usuário clica no botão "Buscar". Ele faz uma solicitação GET para a API de back-end, passando os parâmetros de filtro como parâmetros de consulta e atualiza as variáveis de estado de dados transferencia de acordo.
- O componente inclui vários manipuladores de eventos, como handleInitDate, handleFinDate e handleNomeOperador, para atualizar as variáveis de estado do filtro com base na entrada do usuário.
- O JSX renderizado inclui elementos HTML para exibir as entradas de filtro, o botão de pesquisa, a tabela de transferencia e os controles de paginação.
As linhas da tabela são renderizadas dinamicamente com base nos dados de transferência filtrados, limitados pela página atual e pelos valores limite.
- Os controles de paginação permitem que o usuário navegue pelas páginas de dados de transferência.
Requisitos do Projeto
  # Os requisitos do projeto para o frontend incluem:

- Exibição de dados de transferencia com base nas entradas do filtro (data de inicialização, data de término e nome do operador).
- Calculando e exibindo o saldo total (saldo) e saldo no período selecionado.
- Implementação de paginação com limites configuráveis.
- Estilizando os componentes de acordo com o protótipo fornecido
