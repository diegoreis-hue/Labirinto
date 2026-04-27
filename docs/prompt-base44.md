# Prompt para Base44 - Sistema Labirinto

Crie um sistema web chamado **Labirinto** para controle de inventário, empréstimos e devoluções de materiais dos laboratórios Labirinto, Labin Maker e D03.

O sistema deve ter design tecnológico, moderno e organizado, com fundo escuro, detalhes em dourado e elementos visuais inspirados em placa-mãe, processadores, circuitos e robótica.

## Objetivo

O objetivo do sistema é controlar os materiais dos laboratórios, mostrando quais itens existem, quantos estão disponíveis, quantos estão emprestados e quem está com cada item.

## Estrutura principal

Crie as seguintes áreas:

1. **Tela inicial de escolha do sistema**
   - Mostrar duas opções por logo:
     - Labirinto.
     - Labin Maker.
   - Ao clicar em cada logo, o usuário entra no sistema correspondente.

2. **Login**
   - Criar login com três tipos de usuários:
     - Administrador.
     - Colaborador.
     - Usuário comum.

3. **Dashboard**
   - Mostrar resumo dos materiais.
   - Mostrar total de itens cadastrados.
   - Mostrar itens disponíveis.
   - Mostrar itens emprestados.
   - Mostrar solicitações pendentes.

4. **Inventário**
   - Organizar os materiais por pastas ou categorias.
   - Cada item deve ter:
     - Nome.
     - Descrição.
     - Quantidade total.
     - Quantidade disponível.
     - Quantidade emprestada.
     - Categoria.

5. **Solicitações de empréstimo**
   - Usuário comum pode solicitar um item.
   - Administrador pode aprovar ou recusar.
   - Quando aprovado, a quantidade disponível diminui e a quantidade emprestada aumenta.

6. **Itens emprestados**
   - A quantidade emprestada deve ser clicável.
   - Ao clicar, mostrar quem está com aquele item, a quantidade, data e status.

7. **Devoluções**
   - Usuário solicita devolução.
   - Administrador aprova ou recusa.
   - Quando aprovado, a quantidade disponível aumenta e a emprestada diminui.

8. **Responsáveis**
   - Criar uma aba chamada Responsáveis.
   - Mostrar nome, função, laboratório, e-mail e contato.

9. **Notificações**
   - Enviar avisos por e-mail para novas solicitações, aprovações, recusas e devoluções.

## Permissões

- Administrador pode gerenciar tudo.
- Colaborador pode visualizar e ajudar na organização, mas não deve ter acesso total.
- Usuário comum apenas visualiza, solicita empréstimos e solicita devoluções.

## Banco de dados

Use o banco de dados da própria Base44 ou integração com Supabase, se disponível.

Crie entidades para:

- Usuários.
- Perfis.
- Laboratórios.
- Categorias.
- Itens.
- Empréstimos.
- Devoluções.
- Histórico.
- Responsáveis.

## Regras obrigatórias

- Não permitir empréstimo maior que a quantidade disponível.
- Atualizar as quantidades automaticamente após aprovação.
- Guardar o histórico de empréstimos e devoluções.
- Separar as permissões por tipo de usuário.
- O administrador deve conseguir ver quem pegou cada item.
- O sistema deve funcionar bem em computador e celular.

## Visual

Use um visual limpo, profissional e tecnológico. O sistema deve parecer um projeto real de laboratório de tecnologia, inteligência artificial e robótica.

Cores principais:

- Preto.
- Dourado.
- Cinza escuro.
- Branco para textos importantes.

Evite telas poluídas. Use cards, tabelas, botões e ícones de forma organizada.
