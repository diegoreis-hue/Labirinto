# Especificação do Sistema Labirinto

## 1. Visão geral

O **Labirinto** é um sistema web criado para controlar o inventário dos laboratórios Labirinto, Labin Maker e D03. Ele deve permitir que os responsáveis organizem materiais, acompanhem empréstimos, aprovem solicitações e registrem devoluções.

A proposta é criar uma ferramenta simples de usar, mas completa o suficiente para ajudar no controle real dos equipamentos e materiais dos laboratórios.

## 2. Objetivo do sistema

O objetivo principal é facilitar o armazenamento e o controle dos materiais dos laboratórios, evitando desorganização, perda de itens e falta de informação sobre quem está usando cada material.

O sistema deve mostrar de forma clara:

- Quais materiais existem no laboratório.
- Quantos itens existem no total.
- Quantos estão disponíveis.
- Quantos estão emprestados.
- Quem pegou determinado item emprestado.
- Quais pedidos estão aguardando aprovação.
- Quais devoluções ainda precisam ser confirmadas.

## 3. Tipos de usuários

### Administrador

O administrador tem acesso completo ao sistema. Ele pode cadastrar, editar, excluir e organizar materiais, além de aprovar ou recusar pedidos de empréstimo e devolução.

Permissões principais:

- Gerenciar usuários.
- Criar e editar pastas.
- Cadastrar materiais.
- Alterar quantidades.
- Aprovar empréstimos.
- Aprovar devoluções.
- Visualizar todos os itens emprestados.
- Ver dados completos dos solicitantes.

### Colaborador

O colaborador ajuda na organização do laboratório, mas não possui todas as permissões do administrador.

Permissões principais:

- Visualizar inventário.
- Acompanhar materiais.
- Auxiliar no controle de empréstimos.
- Ver informações permitidas pelo administrador.

### Usuário comum

O usuário comum pode acessar o sistema para visualizar materiais disponíveis e solicitar empréstimos.

Permissões principais:

- Visualizar itens disponíveis.
- Solicitar empréstimos.
- Solicitar devoluções.
- Acompanhar o status dos seus pedidos.

## 4. Módulos do sistema

### 4.1 Login e autenticação

O sistema deve ter login para separar as funções de cada tipo de usuário. Cada pessoa deve acessar apenas o que sua permissão permite.

### 4.2 Inventário

O inventário deve ser organizado por pastas ou categorias. Dentro de cada pasta, devem aparecer os itens cadastrados.

Cada item deve ter:

- Nome.
- Descrição.
- Quantidade total.
- Quantidade disponível.
- Quantidade emprestada.
- Categoria ou pasta.
- Observações, se necessário.

### 4.3 Solicitação de empréstimo

O usuário comum deve poder solicitar o empréstimo de um item. A solicitação deve ficar pendente até ser aprovada por um administrador ou responsável.

Quando o empréstimo for aprovado, o sistema deve atualizar automaticamente a quantidade disponível e a quantidade emprestada.

### 4.4 Controle de itens emprestados

A quantidade emprestada de cada item deve ser clicável. Ao clicar, o administrador deve conseguir ver detalhes como:

- Nome do usuário que pegou o item.
- Item emprestado.
- Quantidade emprestada.
- Data da solicitação.
- Status do empréstimo.
- Informações de contato, se necessário.

### 4.5 Sistema de devolução

A devolução deve seguir uma lógica parecida com a solicitação de empréstimo. O usuário solicita a devolução e o administrador confirma.

Quando a devolução for aprovada, o sistema deve atualizar novamente as quantidades do item.

### 4.6 Aba de responsáveis

O sistema deve ter uma aba chamada **Responsáveis**, mostrando contatos importantes relacionados aos laboratórios.

Essa aba pode conter:

- Nome do responsável.
- Função.
- Laboratório relacionado.
- E-mail.
- Telefone ou outro contato, se for necessário.

### 4.7 Notificações por e-mail

O sistema deve enviar notificações por e-mail para avisar sobre:

- Nova solicitação de empréstimo.
- Aprovação de empréstimo.
- Recusa de empréstimo.
- Solicitação de devolução.
- Aprovação de devolução.

## 5. Integração com Supabase

O projeto deve usar o Supabase como backend, banco de dados e autenticação.

O Supabase pode ser usado para:

- Guardar usuários.
- Guardar materiais.
- Guardar categorias.
- Guardar solicitações.
- Controlar permissões.
- Registrar histórico de empréstimos e devoluções.

## 6. Segundo sistema: Labin Maker

O site deve permitir acesso a outro sistema chamado **Labin Maker**. Esse acesso pode acontecer por uma tela de seleção de logos.

Ao escolher a logo do Labirinto, o usuário entra no sistema Labirinto. Ao escolher a logo do Labin Maker, o usuário entra no sistema do Labin Maker.

O Labin Maker pode ter uma variação de cores para diferenciar os sistemas, mas deve manter a ideia tecnológica.

## 7. Identidade visual

O design deve ser moderno e tecnológico.

Características visuais desejadas:

- Fundo escuro.
- Cores principais: preto e dourado.
- Elementos inspirados em placa-mãe, processador e circuitos.
- Interface organizada e limpa.
- Botões claros e fáceis de entender.
- Aparência profissional, mas simples de usar.

## 8. Regras importantes

- O usuário comum não deve conseguir alterar o inventário.
- Apenas administradores devem aprovar empréstimos e devoluções.
- A quantidade emprestada deve mudar automaticamente após aprovação.
- O sistema deve impedir empréstimos acima da quantidade disponível.
- O histórico de empréstimos deve ser preservado.
- O administrador deve conseguir ver quem está com cada item.
- O sistema deve ser fácil de usar em computador e celular.

## 9. Status do projeto

O projeto ainda está em desenvolvimento e passando por testes com diferentes ferramentas de IA para criação do site, organização visual, geração de logo e escrita da documentação.
