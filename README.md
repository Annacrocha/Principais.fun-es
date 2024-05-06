# Principais.fuções
# GIT e GITHUB
GIT e GITHUB são ferramentas que usadas em conjunto.
O Github é uma “rede social dev” em que é possível armazenar e compartilhar projetos de desenvolvimento de software;é um sistema de controle de versão de arquivos; em outras palavras, é responsável por guardar o histórico de alterações sempre que alguém modificar algum arquivo que está sendo monitorado por ele.

O Git é uma alternativa com um funcionamento mais interessante ainda: ele é distribuído e todo mundo tem uma cópia inteira do repositório, não apenas o "servidor principal", é um sistema de controle de versão distribuído e amplamente adotado.

O Git é um sistema de controle de versão distribuído e amplamente adotado. O Git nasceu e foi tomando espaço dos outros sistemas de controle. Ele se tornou bastante popular por, além de ser um SGVD, se tratar de uma ferramenta de código aberto gratuita, e ser fácil de começar a utilizar. Além disso, trata-se de uma ferramenta muito veloz, devido à sua arquitetura, suporta desenvolvimento não-linear, com milhares de ramificações e funciona muito bem com projetos grandes, afinal, foi pensado para suportar o controle de versões do Linux, um dos sistemas operacionais mais adotados no mundo.

Dentro do GIT encontramos vária ferramentas, como:
 ## Repositórios. commits e árvores (Trees)
 Um repositório é como uma pasta ou diretório que contém todos os arquivos e o histórico de um projeto.

 Já o termo commit pode ter como tradução literal “compromisso”, que seria uma ação em que você faz uma alteração no projeto, se compromete e salva suas alterações no histórico do projeto. Ou seja, cada commit é uma entrada no histórico que contém informações sobre as 
alterações feitas.
 
  Árvores, por último, representam a estrutura do diretório e arquivos em um commit específico, que tem como função registrar a organização do projeto ao longo do histórico de desenvolvimento.
 
 ## Ramificações (Branches) e fusões (Merges)
 As “ramificações” ou branches permitem que você crie linhas separadas de desenvolvimento para trabalhar em recursos ou correções sem afetar a linha principal do projeto.

 Cada branch é uma ramificação independente do código-fonte, possibilitando que você isole e desenvolva novas funcionalidades, refatore o código ou faça correções e testes em paralelo, sem interferir no código existente na branch principal, que geralmente é nomeada como "main".

 Em um projeto com branches diferentes, a fusão, ou merge, permite combinar as alterações dessas branches de volta à linha principal, quando as alterações estão prontas.
 
 ## Controle de versão distribuído
 Existem dois tipos de sistemas de controle de versão. Em um deles, pode haver um único servidor central que armazena o projeto com seu histórico, com o qual as pessoas desenvolvedoras precisam interagir. Isso é característico de um sistema de Controle de Versão Centralizado.

 No outro tipo, cada pessoa desenvolvedora pode manter uma cópia do projeto em sua máquina local, o que é conhecido como Controle de Versão Distribuído, que é o caso do Git.

 Com o Git, cada pessoa desenvolvedora tem uma versão completa do histórico do projeto. Isso proporciona independência e permite o desenvolvimento em paralelo.

## Principais comandos do GIT:

## Git init
É utilizado para inicializar um repositório Git dentro de um diretório do sistema. Após sua utilização, a ferramenta passa a monitorar o estado dos arquivos no projeto.

## Git clone
É utilizado para criar uma cópia de um repositório remoto em um diretório da máquina. Este repositório poder ser criado a partir de um repositório armazenado localmente, através do caminho absoluto ou relativo, ou pode ser remoto, através do URI na rede.
A partir de um repositório clonado, é possível acompanhar o estado de um projeto e suas modificações, além de contribuir com o projeto, a partir do envio das suas modificações ao repositório central.

## Git status
É utilizado para verificar o status de um repositório git, bem como o estado do repositório central. O comando mostra informações sobre se o projeto local está sincronizado com o central, quais arquivos estão sendo monitorados pelo Git e em qual branch você está no projeto.

## Git add
É utilizado para adicionar arquivos ao pacote de alterações a serem feitas. É possível adicionar um único arquivo, múltiplos arquivos de uma vez, como "git add <-arquivo1-> <-arquivo2-> ...", ou até mesmo um diretório, a partir de seu caminho. Uma vez que um arquivo é adicionado ao pacote de alterações com o comando add, ele está pronto para entrar no próximo commit.

## Git commit
É utilizado para criar uma nova versão do projeto a partir de um pacote de alterações. O commit pega o pacote de modificações adicionado através do comando git add, fecha essas alterações num pacote e o identifica através de um Hashcode.
Além disso, para cada commit é necessário escrever uma mensagem para identificá-lo, com uma mensagem clara de quais alterações foram feitas neste commit.

## Git log
É utilizado para ver o histórico de alterações do projeto, onde aparecerão todos os commits feitos, com suas respectivas mensagens e códigos identificadores.
O comando é muito útil quando precisamos rastrear o andamento de um projeto e verificar em qual ponto cada funcionalidade foi implementada.
Além disso, o comando conta com várias opções para mostrar o histórico de forma resumida, gráfica e até mesmo mostrando a diferença entre os commits, que podem ser vistas na documentação oficial do comando.

## Git branch
É utilizado para criar novos ramos de desenvolvimento, bem como visualizar quais são os ramos existentes.
Para criar um novo ramo, basta utilizar o comando git branch seguido do nome do novo ramo, e para visualizar quais os ramos existentes a utilização do comando é bem similar: basta não informar um nome para a nova branch, e serão listadas todas as já criadas.

## Git checkout
É utilizado para navegar entre as versões do projeto, bem como entre as diferentes ramificações criadas.  Para navegar entre as versões, basta usar o comando:
git checkout <- Hashcode do commit ->
E todo o estado do projeto se modificará ao estado no qual o commit foi feito.

Similarmente, para navegar entre as ramificações podemos usar o comando:
git checkout <- nome da branch ->

E a branch será alterada. O comando também permite criar uma branch e imediatamente mudar para ela, através do comando:
git checkout -b <- nome da branch ->
Que vai criar a ramificação e navegar até ela.

## Git diff
É utilizado para visualizar modificações feitas entre commits, sejam eles entre um commit arbitrário e o estado atual do projeto, dois commits arbitrários, ou até mesmo todas alterações entre dois commits distintos.
Para visualizar as alterações entre um commit distinto e o atual, basta usar o comando:
git diff <- Hashcode do commit anterior ->
E serão listadas todas as diferenças no projeto entre os dois commits.

## Git config
É usado para configurar e personalizar o ambiente Git no seu sistema. Ele permite que você defina informações como seu nome de usuário, endereço de e-mail, editor padrão e muitas outras configurações que definem como o Git interage com seus repositórios.
A estrutura básica do comando é:
git config <opções> chave valor

<opções>: Pode ser global (--global) para definir configurações para todos os repositórios no seu sistema ou local (--local) para definir configurações específicas para um repositório em particular.
chave: A chave de configuração que você deseja definir (por exemplo, user.name para o nome de usuário).
valor: O valor que você deseja atribuir à chave (por exemplo, seu nome de usuário ou endereço de e-mail).

Por exemplo, para configurar seu nome de usuário globalmente, você pode usar o comando:

git config --global user.name "Seu Nome"
Isso é útil para garantir que todos os commits que você fizer em qualquer repositório Git no seu sistema tenham o seu nome associado a eles.

Além disso, o comando git config pode ser usado para personalizar muitos outros aspectos do seu ambiente Git, tornando-o mais adaptado às suas preferências e necessidades.

Internamente, o Git cria conjuntos de dados e metadados para armazenar o histórico de um projeto monitorado pela ferramenta.
A esses conjuntos de dados damos o nome de objetos git, e eles podem ser de três tipos:
## Blobs
São objetos criados para armazenar dados de arquivos, porém não guardam seus metadados.
Na prática, a partir do conteúdo de um arquivo é gerado um Hashcode de identificação para ele, que será usado para guardar seu estado em um determinado ponto.
Caso duas pessoas diferentes criem arquivos com exatamente o mesmo conteúdo, o Git criará um blob idêntico para os dois arquivos, pois ele só se baseia no conteúdo do arquivo e não guarda metadados sobre quem criou o arquivo ou quando.
## Trees
São objetos criados para armazenar dados de pastas, como blobs e até mesmo outras trees, podem ser entendidos como a representação de uma pasta dentro do git. Similar ao blob, a tree não guarda metadados e gera um Hashcode de identificação baseado em seu conteúdo.
## Commit
São objetos que guardam o snapshot de um momento do projeto. Dentro de um commit são guardadas trees e blobs, que por sua vez identificam o estado dos arquivos e pastas no momento em que o commit é criado, assim como metadados como quando ele foi criado e por quem.
O Hashcode que identifica um commit é justamente o que aparece ao utilizar o comando git log, e é essencial para controlar as versões do projeto.
## GitHub
GitHub é uma plataforma para gerenciar seu código e criar um ambiente de colaboração entre devs, utilizando o Git como sistema de controle.
Ela vai facilitar o uso do Git, escondendo alguns detalhes mais complicados de setup.
Para se comunicar com o GitHub e mexer nos arquivos do seu repositório, você pode usar o comando do git e suas diretivas de commit, pull e push.
## Conceitos:
 ## Branch:
 Uma ramificação que vai ser feita no projeto, a partir da linha cronológica principal para mudar seu código.

 ## Commit:
 Postar as alterações que foram feitas no projeto, um "marco histórico".

 ## Merge:
 Junção da branch criada com a branch principal.

 ## Remote:
 Vai fazer com que o repositório existente na máquina vá para a plataforma que vai ser utilizada; pegamos o link do repositório que foi criado no GITHUB para poder referenciar.

 ## Push: 
 Utilizado para colocar  COMMIT que foi criado na sua máquina no REMOTE.

 ## Pull:
 Puxa o que está no repositório do GITHUB para sua máquina,ao contrário do PUSH.

 O Github é bastante popular, tanto que é apelidado de rede social da pessoa desenvolvedora, pois além de oferecer os recursos de controle de versão, também é comumente utilizado para compartilhar código e, até mesmo, ser utilizado como um portfólio.
 Projetos de código aberto, ou open source, frequentemente envolvem colaboração de desenvolvedores de todo o mundo, para isso, existem eventos como o Hacktoberfest para incentivar a contribuição da comunidade.
Para garantir a contribuição harmoniosa de diversos colaboradores, geralmente é utilizado o Github com práticas de ramificação e colaboração, como diretrizes para criar forks (bifurcações) que é uma cópia independente do repositório de código-fonte.
Além da convenção de abrir issues (problemas) para discussão e fazer pull requests (solicitações de subir alterações) para propor alterações e revisões de código rigorosas para garantir a qualidade do código.

Mas o Github vai muito além disso: essa tecnologia possui diversas outras ferramentas que otimizam nosso trabalho.
