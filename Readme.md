**Definições e Conceitos importantes**

**Git** é um sistema de controle de versão distribuído, que permite que os desenvolvedores colaborem em projetos de software, gerenciando e rastreando as alterações feitas nos arquivos1. Git é um sistema de controle de versão distribuído, projetado para lidar com tudo, desde projetos pequenos até grandes, com velocidade e eficiência. Ele permite que várias pessoas trabalhem em um projeto simultaneamente, acompanhando as alterações feitas em arquivos ao longo do tempo. Cada usuário tem uma cópia local completa do repositório com histórico completo de alterações, o que permite a colaboração de forma eficiente.

**GitHub** é uma plataforma online que hospeda repositórios Git, facilitando o compartilhamento, o armazenamento e o gerenciamento de código2. Além disso, o GitHub oferece recursos como revisão de código, integração contínua, gerenciamento de projetos, entre outros. GitHub é uma plataforma de hospedagem de código-fonte que utiliza o Git para controle de versão. Ele fornece funcionalidades adicionais, como rastreamento de problemas, solicitações de pull, hospedagem de sites, integração contínua e muito mais. O GitHub torna mais fácil para equipes de desenvolvimento colaborarem em projetos e gerenciarem seu código-fonte de maneira eficiente.

**Principais Comandos do Git/GitHub:**

git init:
Inicia um novo repositório Git.
git clone [URL]:
Clona um repositório existente para o seu computador.
git add [arquivo(s)]:
Adiciona alterações ao stage(etapa) para serem commitadas.
git commit -m "Mensagem do commit":
Registra as alterações no repositório com uma mensagem associada.
git status:
Exibe o status das alterações como não rastreadas, modificadas ou prontas para commit.
git log:
Mostra o histórico de commits.
git push [remote] [branch]:
Envia as alterações locais para o repositório remoto.
git pull [remote] [branch]:
Atualiza o repositório local com as alterações do repositório remoto.
git branch [nome]:
Cria uma nova branch.
git checkout [branch]:
Muda para a branch especificada.
git merge [branch]:
Combina os commits de uma branch com a branch atual.
git remote add [nome] [URL]:
Adiciona um repositório remoto.
git remote -v:
Lista os repositórios remotos associados ao projeto.
git fetch [remote]:
Busca as alterações do repositório remoto, mas não as mescla automaticamente.
git branch -d [branch]:
Deleta uma branch local.

**Pull Requests (PR):**Um Pull Request é um recurso do GitHub que permite que os desenvolvedores solicitem a integração de suas alterações em um repositório Git3. Uma pull request contém as informações sobre as alterações propostas, como o título, a descrição, os commits, os arquivos modificados, os comentários e as revisões. É uma solicitação para mesclar as alterações de uma branch para outra. Geralmente, você cria um Pull Request quando termina de trabalhar em uma feature ou correção de bug em uma branch e deseja mesclar essas alterações de volta à branch principal. Outros membros da equipe revisam o código e, se estiver tudo certo, o Pull Request é aceito e as alterações são mescladas.
Abrir um Pull Request:
Este é geralmente feito através da interface web do GitHub ou GitLab após enviar a branch para o repositório remoto.

Existem algumas **nomenclaturas mais usadas para pull request**, que seguem um padrão de prefixos e sufixos para indicar o tipo, o propósito e o status da solicitação. Alguns exemplos são:

bugfix/ : indica que a pull request está corrigindo um bug no código.
feature/ : indica que a pull request está adicionando um novo recurso ao projeto.
hotfix/ : indica que a pull request está solucionando um problema urgente ou crítico.
improvement/ : indica que a pull request está melhorando algum aspecto do código existente.
WIP : indica que a pull request está em andamento (work in progress) e não está pronta para ser revisada ou mesclada.
RFC : indica que a pull request está solicitando comentários (request for comments) ou feedback dos outros desenvolvedores.
LGTM : indica que a pull request está aprovada (looks good to me) e pode ser mesclada.

**Branchs** são linhas de desenvolvimento paralelas que permitem trabalhar em diferentes funcionalidades, correções ou experimentos sem afetar o branch principal, chamado de master. O Git permite criar, mudar, excluir e mesclar branchs de forma fácil e rápida1.

**Merge:** O Merge é o processo de combinar as alterações de uma branch com outra. Quando um Pull Request é aceito, um Merge é realizado para incorporar as mudanças na branch de destino. São o processo de unir dois ou mais branchs em um só, combinando as alterações feitas em cada um deles. O Git cria um novo commit de merge que tem como pais os commits dos branchs que foram mesclados1.
Fazer o Merge de uma Branch (após revisão do PR):
bash
Copy code
git checkout branch_destino
git merge nome_da_branch

**Conflitos de Merge:**
Conflitos de merge ocorrem quando o Git não consegue realizar automaticamente o merge das alterações devido a alterações conflitantes nas mesmas linhas de código. Nesses casos, o Git solicitará que você resolva os conflitos manualmente antes de finalizar o merge.

A ordem correta de execução depende do fluxo de trabalho que você está seguindo, mas uma forma comum é a seguinte:

Criar um novo branch a partir da master para desenvolver uma nova funcionalidade ou corrigir um bug. O nome do branch deve seguir um padrão que indique o tipo e o propósito da alteração, como feature/, bugfix/, hotfix/, etc3.
Trabalhar no branch criado, fazendo commits regulares e descritivos das alterações. Se necessário, fazer o push do branch para o repositório remoto para compartilhar com outros desenvolvedores ou fazer backup.
Quando o trabalho no branch estiver concluído e testado, fazer o checkout da master e atualizá-la com o repositório remoto, para garantir que ela está sincronizada com as últimas alterações.
Fazer o merge do branch de trabalho na master, resolvendo possíveis conflitos que possam surgir. Se o merge for bem sucedido, fazer o push da master para o repositório remoto, para atualizar a versão de produção.
Criar uma PR no GitHub, solicitando a revisão e o feedback dos outros desenvolvedores sobre as alterações feitas. A PR deve ter um título e uma descrição claros e informativos, e seguir as boas práticas de código e estilo2.
Aguardar a aprovação da PR, respondendo aos comentários e sugestões que possam surgir. Se necessário, fazer alterações no branch de trabalho e atualizar a PR. Se a PR for aprovada, fazer o merge dela na master e deletar o branch de trabalho.

Observação: Markdown é uma linguagem de marcação que permite formatar textos na web de forma simples e rápida. Ela é usada no GitHub para criar arquivos README, pull requests, issues e wikis, entre outros. Com Markdown, você pode adicionar elementos como títulos, listas, links, imagens, tabelas, código, etc., usando apenas caracteres especiais, como #, *, e []. Markdown facilita a leitura e a escrita de textos na web, tornando-os mais organizados e apresentáveis. 

Links que podem ajudar
1 docs.github.com
2 brunodulcetti.com
3 medium.com
4 github.com
5 git-scm.com

Próximos tópicos
Exercícios de lógica de programação
Conceito OOP e aplicação em projetos
Estudos dos comandos básicos de SQL (create, delete, insert, update, select, alter)
