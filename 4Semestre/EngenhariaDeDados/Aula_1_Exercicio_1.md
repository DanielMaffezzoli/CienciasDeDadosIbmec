# Minimundo: Gerenciamento de um Projeto

Uma empresa deseja implementar um sistema para gerenciar os usuários e suas interações em um projeto colaborativo. O sistema deve permitir o cadastro de informações sobre os usuários, seus cargos e as salas onde eles podem acessar recursos específicos. Além disso, é necessário controlar as permissões de cada cargo para garantir que os usuários tenham acesso apenas às funcionalidades adequadas ao seu perfil.

Cada usuário do sistema possui um nome, um endereço de email e um cargo associado. O cargo define o nível de acesso do usuário no sistema e especifica quais salas ele pode acessar, além de listar as permissões concedidas. As permissões incluem a capacidade de editar, deletar ou visualizar os recursos disponíveis nas salas autorizadas. Cada sala possui um nome único e um código identificador, que são utilizados para organizar os recursos do projeto.

O sistema deve garantir que os usuários só tenham acesso às salas autorizadas pelo seu cargo. Além disso, as permissões de cada cargo devem ser respeitadas para evitar acessos indevidos. Essas regras são essenciais para manter a segurança e a organização do projeto, garantindo que cada colaborador possa desempenhar suas funções dentro dos limites estabelecidos.

---

## Elementos Principais

### Usuário
Representa os colaboradores do projeto. Para cada usuário, é necessário armazenar:
- Nome
- Email
- Cargo

### Cargo
Define o papel de um usuário no sistema. Cada cargo possui:
- Nome
- Lista de salas autorizadas
- Permissões associadas:
  - Editar
  - Deletar
  - Visualizar

### Sala
Representa os ambientes onde os recursos do projeto estão organizados. Cada sala possui:
- Nome (único)
- Código identificador

---

## Regras de Negócio

1. Um usuário só pode acessar as salas autorizadas pelo seu cargo.
2. As permissões de um cargo determinam as ações que o usuário pode realizar nas salas autorizadas.
3. Cada sala deve ter um nome único e um código identificador para facilitar a organização dos recursos.
