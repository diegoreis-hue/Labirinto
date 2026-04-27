# Prompt Principal para Criação do Site Labirinto

Crie um sistema web completo chamado **Labirinto**, voltado para controle de inventário, empréstimos e devoluções de materiais dos laboratórios Labirinto, Labin Maker e D03.

O sistema deve ter uma aparência tecnológica, moderna e organizada, com identidade visual inspirada em placa-mãe, processador, circuitos, robótica e laboratório de inteligência artificial. Use principalmente as cores **preto e dourado**.

## Objetivo do site

O site deve permitir que os responsáveis pelos laboratórios cadastrem materiais, organizem itens por pastas, controlem quantidades disponíveis e emprestadas, aprovem solicitações de empréstimo, registrem devoluções e acompanhem quem está com cada material.

## Tipos de usuários

Crie três tipos de usuários:

1. **Administrador**
   - Acesso total ao sistema.
   - Pode cadastrar, editar e excluir materiais.
   - Pode criar e editar pastas.
   - Pode aprovar ou recusar empréstimos.
   - Pode aprovar ou recusar devoluções.
   - Pode visualizar quem está com cada item emprestado.
   - Pode gerenciar responsáveis e usuários.

2. **Colaborador**
   - Pode visualizar o inventário.
   - Pode acompanhar materiais e ajudar na organização.
   - Deve ter permissões menores que o administrador.

3. **Usuário comum**
   - Pode visualizar materiais disponíveis.
   - Pode solicitar empréstimos.
   - Pode solicitar devoluções.
   - Pode acompanhar o status dos seus pedidos.

## Funcionalidades principais

- Login e autenticação com controle de permissões.
- Dashboard inicial com resumo do inventário.
- Pastas ou categorias para organizar os materiais.
- Cadastro de itens com nome, descrição, quantidade total, quantidade disponível e quantidade emprestada.
- Sistema de solicitação de empréstimo.
- Tela para o administrador aprovar ou recusar empréstimos.
- Atualização automática das quantidades quando um empréstimo for aprovado.
- A quantidade emprestada deve ser clicável.
- Ao clicar na quantidade emprestada, mostrar uma lista com os usuários que estão com aquele item.
- Sistema de solicitação de devolução.
- Tela para o administrador aprovar ou recusar devoluções.
- Atualização automática das quantidades após a devolução aprovada.
- Histórico de empréstimos e devoluções.
- Aba chamada **Responsáveis**, com nome, função, laboratório, e-mail e contato dos responsáveis.
- Notificações por e-mail para pedidos, aprovações, recusas e devoluções.

## Banco de dados e backend

Use **Supabase** para autenticação, banco de dados e armazenamento das informações.

Crie tabelas para:

- Usuários.
- Perfis e permissões.
- Laboratórios.
- Pastas ou categorias.
- Itens do inventário.
- Solicitações de empréstimo.
- Solicitações de devolução.
- Histórico.
- Responsáveis.

## Regras importantes

- Usuário comum não pode alterar inventário.
- Colaborador não deve ter acesso total igual ao administrador.
- Administrador pode visualizar todos os dados.
- O sistema deve impedir empréstimos maiores que a quantidade disponível.
- A quantidade disponível deve diminuir quando o empréstimo for aprovado.
- A quantidade emprestada deve aumentar quando o empréstimo for aprovado.
- A quantidade disponível deve aumentar quando a devolução for aprovada.
- A quantidade emprestada deve diminuir quando a devolução for aprovada.
- O histórico não deve ser apagado.

## Tela de escolha de sistema

Antes de entrar no sistema, crie uma tela de seleção com logos para escolher entre:

- Labirinto.
- Labin Maker.

Ao clicar na logo do Labirinto, abrir o sistema Labirinto. Ao clicar na logo do Labin Maker, abrir o sistema Labin Maker.

O Labin Maker pode usar uma variação de cores, mas deve manter a ideia tecnológica.

## Design

O design deve ser:

- Profissional.
- Moderno.
- Tecnológico.
- Fácil de entender.
- Responsivo para computador e celular.
- Com fundo escuro e detalhes em dourado.
- Com cards, tabelas e botões bem organizados.

Use elementos visuais que lembrem circuitos, processadores, laboratório, tecnologia e robótica, mas sem deixar a tela poluída.

## Resultado esperado

Entregue um site funcional, organizado, bonito e preparado para ser usado como sistema real de controle dos laboratórios.
