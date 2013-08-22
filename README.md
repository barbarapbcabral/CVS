CVS

sistema de controle de versão CVS.

CVS utiliza uma arquitetura cliente-servidor: um servidor armazena a(s) versão(ões) atuais do projeto e seu histórico, e os clientes se conectam a esse servidor para obter uma cópia completa do projeto, trabalhar nessa cópia e então devolver suas modificações. Tipicamente, cliente e servidor devem estar conectados por uma rede local de computadores, ou pela Internet, mas o cliente e o servidor podem estar na mesma máquina se a configuração do CVS for feita de maneira a dar acesso a versões e histórico do projeto apenas a usuários locais. O servidor geralmente roda sistema ao estilo Unix, enquanto o cliente CVS pode rodar qualquer sistema operacional.


Vários clientes podem editar cópias do mesmo projeto de maneira concorrente. Quando eles confirmam suas alterações, o servidor tenta fazer uma fusão delas. Se isso não for possível, por exemplo porque mais de um cliente tentou executar alterações na mesma linha do documento, o servidor apenas executa a primeira alteração e informa ao responsável pela segunda alteração que houve conflito, e que é necessário uma intervenção humana. Se a validação da alteração for bem sucedida, o número de versão de cada cliente arquivo envolvido é incrementado, e o servidor CVS escreve uma linha de observação (fornecida pelo usuário), a data e o autor das alterações em seus arquivos de log.
