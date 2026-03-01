Repositórios Remotos, Push, Pull, Clone, Branch e Merge
1. Introdução ao Trabalho Colaborativo com Git
No primeiro encontro, aprendemos os conceitos básicos do Git e como gerenciar um repositório local.
Agora, vamos explorar o poder do Git para o trabalho em equipe. Os repositórios remotos são a peça-chave
para a colaboração, permitindo que múltiplos desenvolvedores trabalhem no mesmo projeto de forma
sincronizada e organizada.
2. Repositórios Remotos
Um repositório remoto é uma versão do seu projeto que está hospedada na internet ou em uma rede. O
mais comum é utilizar serviços como o GitHub, GitLab ou Bitbucket. Ter um repositório remoto permite
que você:
• Colabore com outras pessoas: Vários desenvolvedores podem contribuir para o mesmo projeto.
• Faça backup do seu código: Seu código fica seguro em um servidor externo.
• Acesse seu projeto de qualquer lugar: Você pode clonar seu repositório em diferentes máquinas.
2.1.Configurando um Repositório Remoto
Para conectar seu repositório local a um repositório remoto, você utiliza o comando git remote add.
Geralmente, o nome padrão para o repositório remoto principal é origin.
Figura 1: Diagrama conceitual de repositório remoto Git.
A figura acima mostra a conexão entre o repositório local (em sua máquina) e o repositório remoto (no
servidor), ilustrando como a sincronização bidirecional permite colaboração e backup do código.
Exemplo: comando para adicionar um repositório remoto chamado 'origin' com a URL especificada
git remote add origin https://github.com/seu-usuario/seu-repositorio.git

Repositórios Remotos, Push, Pull, Clone, Branch e Merge

Sincronizando com o Repositório Remoto: Push, Pull e Clone


Push envia commits locais, pull recebe mudanças remotas e clone copia um repositório completo. Cada
operação tem direção e propósito específicos.

git push: Enviando Alterações

O comando git push é usado para enviar seus commits locais para o repositório remoto. É assim que você
compartilha suas contribuições com a equipe.

Exemplo: comando para enviar os commits do seu branch local 'main' para o repositório remoto 'origin'
git push origin main

git pull: Recebendo Alterações

O comando git pull é usado para buscar e baixar o conteúdo de um repositório remoto e atualizar seu
repositório local para que ele corresponda a esse conteúdo. É uma combinação dos comandos git fetch e
git merge.

Exemplo: comando para baixar as alterações do branch 'main' do repositório remoto 'origin' e as mescla ao
seu branch local
git pull origin main

git clone: Clonando um Repositório
O comando git clone é usado para criar uma cópia local de um repositório remoto existente. Ele baixa
todo o histórico do projeto e cria uma conexão com o repositório remoto, que por padrão é chamada de
origin.

Exemplo: comando para clonar o repositório especificado para um diretório local chamado meu_diretorio.
git clone https://github.com/usuario/repositorio.git meu_diretorio

Trabalhando com Branches: branch e merge

Branches (ramificações) são uma das características mais poderosas do Git. Eles permitem que você
desenvolva funcionalidades, corrija bugs ou experimente novas ideias em uma linha de desenvolvimento
isolada, sem afetar o código principal (geralmente no branch main ou master).

Diagrama visual do fluxo de trabalho com branches no Git.
A figura acima mostra como criar um branch, desenvolver nele e depois fazer merge de volta ao branch
principal. As linhas representam o histórico de commits e as setas mostram o fluxo de desenvolvimento.

git branch: Gerenciando Branches

O comando git branch permite criar, listar e excluir branches.
Exemplos:
a) Lista todos os branches locais
git branch
b) Cria um novo branch chamado 'nova-funcionalidade'
git branch nova-funcionalidade
c) Muda para o branch 'nova-funcionalidade'
git checkout nova-funcionalidade
d) Cria e muda para um novo branch em um único comando
git checkout -b outra-funcionalidade

git merge: Mesclando Branches

Depois de concluir o trabalho em um branch, você pode mesclar (integrar) suas alterações de volta ao
branch principal usando o comando git merge. O merge combina o histórico de dois ou mais branches.
Exemplo: suponha que você terminou o trabalho no branch nova-funcionalidade e quer integrá-lo ao
main.
a) Primeiro, volte para o branch principal.
git checkout main
b) Agora, mescle o branch 'nova-funcionalidade' no 'main'
git merge nova-funcionalidade

Repositórios Remotos, Push, Pull, Clone, Branch e Merge

Conflitos de Merge

Às vezes, o Git não consegue mesclar as alterações automaticamente. Isso acontece quando duas pessoas
modificam a mesma linha de um arquivo em branches diferentes. Isso é chamado de conflito de merge.
Quando um conflito ocorre, o Git pausa o processo de merge e marca o arquivo conflitante. Você precisa
resolver o conflito manualmente, editando o arquivo para escolher quais alterações manter, e então
finalizar o merge.
