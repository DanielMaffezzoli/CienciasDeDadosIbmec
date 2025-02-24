# Minimundo: Gerenciamento de Equipe em uma Empresa de Software

Uma empresa de desenvolvimento de software deseja implementar um sistema para gerenciar os membros da equipe e suas interações em projetos de tecnologia. O sistema deve permitir o cadastro de informações sobre os colaboradores, seus cargos e os repositórios de código ou áreas de trabalho aos quais eles têm acesso. Além disso, é necessário controlar as permissões de cada cargo para garantir que os colaboradores só possam interagir com os recursos de acordo com suas responsabilidades.

Cada colaborador possui um nome, um endereço de email e um cargo associado. O cargo define o nível de acesso no sistema e especifica quais repositórios ou áreas de trabalho ele pode acessar, além de listar as permissões associadas. As permissões incluem a capacidade de editar código, aprovar mudanças ou apenas visualizar os recursos nos repositórios permitidos. Cada repositório tem um nome único e um identificador, usados para organizar os projetos da empresa.

O sistema deve assegurar que os colaboradores só acessem os repositórios autorizados pelo seu cargo, e que as permissões sejam rigorosamente aplicadas para evitar alterações indevidas ou vazamento de informações. Essas regras são fundamentais para manter a segurança dos projetos e a eficiência da equipe, permitindo que cada colaborador contribua dentro de seus limites definidos.

## Elementos Principais

### Colaborador
Representa os membros da equipe da empresa. Para cada colaborador, é necessário armazenar:

- **Nome**
- **Email**
- **Cargo**

### Cargo
Define o papel de um colaborador na empresa. Cada cargo possui:

- **Nome** (ex.: Desenvolvedor, Gerente de Projeto, Analista de Qualidade)
- **Lista de repositórios autorizados**
- **Permissões associadas:**
  - **Editar** (modificar código ou documentos)
  - **Aprovar** (revisar e liberar mudanças)
  - **Visualizar** (acesso apenas leitura)

### Repositório
Representa os espaços onde os códigos e recursos dos projetos estão armazenados. Cada repositório possui:

- **Nome** (único, ex.: "AppMobile_v2")
- **Identificador** (ex.: "REP-001")

## Regras de Negócio

1. Um colaborador só pode acessar os repositórios autorizados pelo seu cargo.
2. As permissões de um cargo determinam as ações que o colaborador pode realizar nos repositórios autorizados (ex.: um Desenvolvedor pode editar, mas um Analista de Qualidade só aprova ou visualiza).
3. Cada repositório deve ter um nome único e um identificador para facilitar o rastreamento e a organização dos projetos.
