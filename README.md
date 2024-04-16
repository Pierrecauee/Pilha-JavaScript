Sistema de Controle de Atendimento
Este é um sistema de controle de atendimento simples, implementado em JavaScript, que utiliza uma fila circular para gerenciar os pacientes em espera.

Estrutura do Projeto
index.html: O arquivo HTML que contém a estrutura da página web e os elementos de interface do usuário.
FilaCircular.js: Implementação da classe FilaCircular, responsável por gerenciar a fila de pacientes.
index.js: Arquivo JavaScript principal que contém as funções para interagir com a fila e atualizar a interface do usuário.
atendimento.js: Outro arquivo JavaScript que contém as funções relacionadas ao atendimento, como obter a data e a hora atuais e calcular a diferença entre horas.
Funcionalidades

Adicionar Paciente
A função adicionarElemento() permite adicionar um paciente à fila. Ela extrai os valores dos campos de entrada de nome e CPF do HTML, cria um objeto representando o paciente e o adiciona à fila utilizando o método enqueue() da classe FilaCircular.

Remover Paciente
A função removerElemento() remove o primeiro paciente da fila, representando o paciente que foi atendido. Ela utiliza o método dequeue() da classe FilaCircular para remover o paciente da fila.

Buscar por CPF
A função buscarCpf() permite buscar um paciente na fila pelo seu CPF. Ela extrai o valor do campo de entrada do CPF do HTML e utiliza o método buscarPorCpf() da classe FilaCircular para encontrar a posição do paciente na fila.

Atualizar a Exibição da Fila
A função atualizarFila() atualiza a exibição da fila na interface do usuário. Ela limpa a lista de pacientes atualmente exibida e preenche-a com os pacientes atuais da fila. Além disso, atualiza o texto indicando o número total de pacientes na fila.
