# Git workflow

## Visão geral do Git workflow

Workflow é a definição, execução e automação de como se da o fluxo de tarefas, informações ou documentos que são passados ​​de um participante para outro dentro do ciclo de vida de um projeto.


## Vantagens Git workflow

1. Por mais que possa parecer complicado de entender a princípio, adotar o uso do Git workflow torna o fluxo de trabalho git fácil de compreender, o que garante produtividade máxima em um período de tempo menor.

2. Fornece uma padronização de trabalho e comandos, facilitando a implementação. Adota um padrão semelhante para todas as três categorias de branchs, garantindo erros mínimos no que diz respeito ao desenvolvimento ou operações de desenvolvimento.


## Introdução a alguns workflows mais utilizados

### 1. **Github Workflow**

#### 1.1 Criar um branch

   Crie um branch no seu repositório. Um nome de branch curto e descritivo permite que seus colaboradores vejam o trabalho em andamento rapidamente. Por exemplo, `increase-test-timeout` ou `add-code-of-conduct`.

#### 1.2. Fazer alterações

No seu branch, faça quaisquer alterações desejadas no repositório.

Seu branch é um lugar seguro para fazer alterações. Se você cometer um erro, você poderá reverter suas alterações ou fazer push das alterações adicionais para corrigir o erro. As suas alterações não serão feitas no branch padrão até que você faça merge de seu branch.

Faça o commit e faça push das alterações no seu branch. Dê a cada commit uma mensagem descritiva para ajudar você e futuros contribuidores a entender quais alterações o commit contém. Por exemplo, fix typo ou increase rate limit.

Idealmente, cada commit contém uma alteração isolada e completa. Isso facilita reverter as suas alterações se decidirmos adotar uma abordagem diferente. Por exemplo, se você deseja renomear uma variável e adicionar alguns testes, coloque a variável renomeada em um commit e os testes em outro commit. Posteriormente, se você quiser manter os testes, mas reverter o novo nome da variável, você poderá reverter o commit específico que continha a variável renomeada. Se você colocar o novo nome da variável e testar no mesmo commit ou espalhar o novo nome da variável por múltiplos commits, você gastaria mais esforço revertendo suas alterações.

Ao fazer commit e push das suas alterações, você fará backup do seu trabalho no armazenamento remoto. Isso significa que você pode acessar seu trabalho a partir de qualquer dispositivo. Isso também significa que os seus colaboradores poderão ver o seu trabalho, responder a perguntas e fazer sugestões ou contribuições.

Continue a criar, fazer commit e fazer push das alterações no seu branch até que você esteja pronto para pedir feedback.

#### 1.3. Criar uma solicitação de pull
    
Crie um pull request para pedir aos colaboradores feedback sobre suas alterações. A revisão de pull request é tão valiosa que alguns repositórios exigem uma revisão de aprovação antes que os pull requests possam ser mesclados. Se você quiser feedback ou conselhos antes de concluir suas alterações, você poderá marcar seu pull request como um rascunho. 

Ao criar uma pull request, inclua um resumo das alterações e qual o problema que elas resolvem. Você pode incluir imagens, links e tabelas para ajudar a transmitir estas informações. Se o seu pull request resolve um problema, vincule o problema para que os interessados no problema estejam cientes do pull request e vice-versa. Se você vincular com uma palavra-chave, o problema será fechado automaticamente quando o pull request for mesclado.

Além de preencher o texto do pull request, você pode adicionar comentários em linhas específicas do pull request para apontar algo explicitamente para os revisores.

Seu repositório pode ser configurado para solicitar uma revisão automaticamente de equipes específicas ou usuários quando um pull request for criado. Você também pode @mention manualmente ou solicitar uma revisão de pessoas ou de equipes específicas.

Se seu repositório tiver verificações configuradas para serem executadas em pull requests, você verá todas as verificações que falharam no seu pull request. Isso ajuda você a capturar erros antes de fazer merge do seu branch. 

#### 1.4. Fazer merge do seu pull request

Depois que seu pull request for aprovado, faça merge do seu pull request. Isso fará o merge automático do seu branch para que suas alterações apareçam no branch padrão. GitHub mantém o histórico de comentários e commits no pull request para ajudar futuros contribuidores a entender suas alterações. 

GitHub dirá se o seu pull request possui conflitos que precisam ser resolvidos antes do merge.

Configurações de proteção de branch podem bloquear o merge se seu pull request não cumprir certos requisitos. Por exemplo, você precisa de um certo número de revisões ou uma revisão de aprovação de uma equipe específica. 

