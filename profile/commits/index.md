O Padrão de Commits é uma convenção adotada pela comunidade de desenvolvimento de software para padronizar as mensagens de commit usadas ao versionar um projeto no controle de versão, como o Git. Essas mensagens descrevem as alterações feitas em cada commit e ajudam a manter um histórico de alterações claro e compreensível.

Uma das implementações populares do Padrão de Commits é conhecida como **Conventional Commits** *(Commits Convencionais)*. O **Conventional Commits** define um conjunto de regras para a formatação das mensagens de commit, permitindo que desenvolvedores e equipes mantenham um registro consistente e estruturado do trabalho realizado. O formato geral das mensagens de commit no **Conventional Commits** segue o padrão:

```
<tipo>[escopo opcional]: <descrição>
```
O **tipo** indica a natureza do commit, podendo ser:
- **feat**: para introduzir uma nova funcionalidade;
- **fix**: para correção de bugs;
- **docs**: para atualizações de documentação;
- **style**: para mudanças que não afetam o código em si (como formatação, espaçamento, etc.);
- **refactor**: para alterações de código que não corrigem bugs nem adicionam novas - funcionalidades;
- **test**: para adicionar ou modificar testes;
- **chore**: para alterações relacionadas a tarefas de construção, ferramentas, etc.

O **escopo opcional** é usado para fornecer um contexto adicional sobre a alteração, como o módulo ou componente específico afetado.

A **descrição** é uma breve explicação sobre a alteração realizada no commit.

<hr />

A adoção do Padrão de Commits e do **Conventional Commits** pode trazer benefícios significativos para a colaboração em projetos, pois facilita a leitura e a compreensão do histórico de alterações. Além disso, ferramentas de automação podem aproveitar esse padrão para realizar ações específicas com base no tipo de commit, como gerar notas de lançamento automaticamente, executar testes relevantes, entre outros.

**Husky** é uma ferramenta popular usada em projetos do Git para automatizar a execução de scripts antes de determinados eventos, como um commit ou push. Ele permite definir ganchos *(hooks)* personalizados que são acionados automaticamente para realizar tarefas específicas. No contexto dos commits convencionais, o **Husky** é frequentemente usado para garantir que as mensagens de commit sigam o formato correto do **Conventional Commits**.

**Commit lint** é uma biblioteca que pode ser usada juntamente com o **Husky** para validar as mensagens de commit em relação às regras definidas pelo **Conventional Commits**. Ele pode verificar se o formato está correto, se o tipo de commit é válido e se o escopo está sendo usado adequadamente. Dessa forma, o **Commit lint** ajuda a manter a consistência e a conformidade das mensagens de commit no projeto.