CVS

sistema de controle de versão CVS.

CVS utiliza uma arquitetura cliente-servidor: um servidor armazena a(s) versão(ões) atuais do projeto e seu histórico, e os clientes se conectam a esse servidor para obter uma cópia completa do projeto, trabalhar nessa cópia e então devolver suas modificações. Tipicamente, cliente e servidor devem estar conectados por uma rede local de computadores, ou pela Internet, mas o cliente e o servidor podem estar na mesma máquina se a configuração do CVS for feita de maneira a dar acesso a versões e histórico do projeto apenas a usuários locais. O servidor geralmente roda sistema ao estilo Unix, enquanto o cliente CVS pode rodar qualquer sistema operacional.


Vários clientes podem editar cópias do mesmo projeto de maneira concorrente. Quando eles confirmam suas alterações, o servidor tenta fazer uma fusão delas. Se isso não for possível, por exemplo porque mais de um cliente tentou executar alterações na mesma linha do documento, o servidor apenas executa a primeira alteração e informa ao responsável pela segunda alteração que houve conflito, e que é necessário uma intervenção humana. Se a validação da alteração for bem sucedida, o número de versão de cada cliente arquivo envolvido é incrementado, e o servidor CVS escreve uma linha de observação (fornecida pelo usuário), a data e o autor das alterações em seus arquivos de log.

Clientes podem comparar diferentes versões de um arquivo, pedir um histórico completo das alterações, ou baixar uma determinada versão do projeto, ou de uma data específica, não necessariamente a versão mais atual. Muitos projetos de código aberto permitem acesso para leitura anônimo, o que significa que qualquer pessoa pode baixar ou comparar versões sem necessidade de autenticação; somente para salvar mudanças é necessário informar a senha nesses casos.

Clientes também podem usar o comando "update" para manter suas cópias locais atualizadas com a última versão do servidor. Isso elimina a necessidade de se fazer diversos downloads de todo o projeto


O CVS também pode manter diferentes "estados" do projeto. Por exemplo, uma versão do software pode ser um desses estados, usado para correção de bugs, enquanto outra versão, que está realmente sob desenvolvimento, sofrendo alterações e tendo novas funcionalidades implementadas, forma o outro estado.

O CVS usa compressão delta para armazenar de maneira eficiente diferentes versões de um mesmo arquivo.
