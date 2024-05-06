# Principais.fuções
# GIT e GITHUB
GIT e GITHUB são ferramentas que usadas em conjunto.
O Github é uma “rede social dev” em que é possível armazenar e compartilhar projetos de desenvolvimento de software;é um sistema de controle de versão de arquivos; em outras palavras, é responsável por guardar o histórico de alterações sempre que alguém modificar algum arquivo que está sendo monitorado por ele.
É uma alternativa com um funcionamento mais interessante ainda: ele é distribuído e todo mundo tem uma cópia inteira do repositório, não apenas o "servidor principal".O Git é uma alternativa com um funcionamento mais interessante ainda: ele é distribuído e todo mundo tem uma cópia inteira do repositório, não apenas o "servidor principal", é um sistema de controle de versão distribuído e amplamente adotado.
O Git se tornou bastante popular por, além de ser um SGVD, se tratar de uma ferramenta de código aberto gratuita, e ser fácil de começar a utilizar. Além disso, trata-se de uma ferramenta muito veloz, devido à sua arquitetura, suporta desenvolvimento não-linear, com milhares de ramificações e funciona muito bem com projetos grandes, afinal, foi pensado para suportar o controle de versões do Linux, um dos sistemas operacionais mais adotados no mundo.
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

