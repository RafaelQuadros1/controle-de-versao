# 📚 Guia de Boas Práticas no Git e Commits

Este guia reúne boas práticas para o uso do Git e a criação de commits organizados e claros. O objetivo é facilitar o trabalho em equipe, minimizar conflitos e garantir que o histórico do projeto seja útil e fácil de entender.

---

## 🎯 **Objetivo**
Promover a produtividade e a colaboração eficiente com um repositório organizado, rastreável e bem documentado.

---

## 🛠️ **Configurações Básicas do Git**

1. Configure seu nome e e-mail globais antes de começar:
   ```bash
   git config --global user.name "Seu Nome"
   git config --global user.email "seuemail@exemplo.com"
   ```
2. Escolha um editor padrão para mensagens de commit:
   ```bash
   git config --global core.editor "seu_editor_preferido"
   ```

---

## 🌟 **Boas Práticas no Git**

### 1. **Organização dos Commits**
- **Commits Pequenos e Frequentes**: Divida mudanças grandes em partes menores e faça commits frequentemente.
- **Mensagens de Commit Claras**: Explique de forma objetiva o que foi feito e, se necessário, por quê. 

#### Estrutura Ideal de Mensagens de Commit
```plaintext
<tipo>: Mensagem breve explicando a mudança

Descrição detalhada, se necessário, explicando o motivo ou contexto
```

##### Exemplos de Tipos:
- **feat**: Adição de nova funcionalidade.
  ```plaintext
  feat: adicionar funcionalidade de login
  ```
- **fix**: Correção de bug.
  ```plaintext
  fix: corrigir erro no cálculo de desconto
  ```
- **docs**: Atualizações na documentação.
  ```plaintext
  docs: atualizar README com instruções de instalação
  ```
- **style**: Alterações visuais ou de formatação.
  ```plaintext
  style: corrigir espaçamento em código CSS
  ```
- **refactor**: Refatoração de código sem alterar funcionalidades.
  ```plaintext
  refactor: melhorar estrutura do método calcularTotal()
  ```

---

### 2. **Uso de Branches**
- Crie uma nova branch para cada funcionalidade ou correção:
  ```bash
  git checkout -b nome-da-branch
  ```
- **Nomeie Branches de Forma Significativa**:
  - `feat/nova-funcionalidade`
  - `fix/corrigir-bug`
- **Finalize Antes de Mesclar**: Teste o código e garanta que ele esteja pronto antes de abrir um pull request.

---

### 3. **Gerenciamento de Merges**
- **Prefira Pull Requests**: Permita que as mudanças sejam revisadas antes de serem mescladas.
- **Revisão de Código**: Sempre peça feedback para evitar erros e manter a qualidade do código.
- **Evite Commits Diretos na Branch Principal**.

---

### 4. **Sincronização e Organização**
- **Sincronize Antes de Trabalhar**: Sempre puxe as mudanças mais recentes antes de começar:
  ```bash
  git pull origin main
  ```
- **Use o .gitignore**: Exclua arquivos desnecessários para manter o repositório limpo.
  Exemplo:
  ```
  # Arquivos temporários
  *.log
  *.tmp

  # Dependências
  node_modules/

  # Configurações de IDE
  .vscode/
  ```

---

## 📝 **Boas Práticas para Commits**

### 1. **Escreva Mensagens no Imperativo**
- Use verbos como "adicionar", "corrigir" ou "remover".
  - Exemplo correto: `feat: adicionar funcionalidade de busca`
  - Exemplo errado: `adicionando funcionalidade de busca`

### 2. **Seja Específico**
- Descreva exatamente o que mudou e evite mensagens genéricas como "atualizações" ou "mudanças feitas".

### 3. **Contextualize, se Necessário**
- Adicione uma descrição detalhada para explicar mudanças complexas.
  ```plaintext
  fix: corrigir erro na validação de e-mail

  O erro ocorria quando o usuário utilizava um e-mail com domínio personalizado.
  Resolves: #123
  ```

---

## 👥 **Trabalho em Equipe**

1. **Defina um Fluxo de Trabalho**: Combine com a equipe um modelo como Git Flow ou GitHub Flow.
2. **Comunique Mudanças**: Antes de subir alterações grandes, avise os colegas para evitar conflitos.
3. **Revisão Coletiva**: Participe das revisões de pull requests para melhorar a qualidade do código.

---

## 📌 **Checklist de Boas Práticas**

Antes de criar um commit ou pull request:
- ✅ A mudança está pequena e lógica?
- ✅ Testei meu código antes de commitar?
- ✅ A mensagem do commit reflete claramente a alteração?
- ✅ O repositório está sincronizado?
- ✅ Não incluí arquivos desnecessários?

---

## 🚀 **Conclusão**
Seguindo estas boas práticas, você terá um repositório limpo, organizado e fácil de trabalhar, seja individualmente ou em equipe. Com isso, as chances de sucesso no projeto aumentam significativamente. 🎉

Bons commits e boa codificação! 😎
