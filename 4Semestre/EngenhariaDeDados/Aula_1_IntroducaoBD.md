# Resumo: Introdução à Banco de Dados

## Conceitos Fundamentais de Banco de Dados
- **Dados**: Fatos conhecidos que podem ser armazenados e possuem significado implícito.
- **Banco de Dados (BD)**:
  - Coleção logicamente coerente de dados relacionados.
  - Representa algum aspecto do mundo real (mini-mundo ou Universo do Discurso).
  - Mudanças no mini-mundo são refletidas no banco de dados.
  - Projetado, construído e populado com dados para um propósito específico.
  - Possui um grupo específico de usuários e aplicações preestabelecidas.

---

## Pirâmide do Conhecimento
1. **Dado**:
   - Elementos não interpretados, observações, fatos ou características.
   - Exemplos: "hoje é sexta", "12 graus Celsius".
2. **Informação**:
   - Dados que possuem significado em um contexto específico.
   - Exemplo: "40 graus Celsius no Rio de Janeiro".
3. **Conhecimento**:
   - Interpretação formal das relações entre dados e informação.
   - Exemplo: "Se a umidade relativa do ar está em 95%, vai chover".
4. **Sabedoria**:
   - Integração e evolução de múltiplos domínios de conhecimento ao longo do tempo.
   - Permite prever tendências e desenvolver novas teorias.

---

## Sistemas de Gerenciamento de Banco de Dados (SGBD)
- **Definição**:
  - Coleção de programas que possibilitam a criação e manutenção de um banco de dados.
  - Software de uso geral, não direcionado a nenhum tipo de aplicação específica.
- **Funcionalidades**:
  - Definir um BD: especificar tipos de dados, estruturas e restrições.
  - Construir um BD: armazenar dados em meio de armazenamento manipulado pelo SGBD.
  - Manipular um BD: busca, modificação de dados e geração de relatórios.

---

## Características Desejáveis em um SGBD
- **ACID** (Atomicidade, Consistência, Isolamento, Durabilidade).
- Persistência de objetos.
- Controle de redundância.
- Manutenção de restrições de integridade.
- Representação de relacionamentos complexos entre os dados.
- Restrições de acesso.
- Múltiplas interfaces para o usuário.
- Realização de inferências utilizando regras de dedução.
- Rotinas para backup e recuperação dos dados.

---

## Metadados
- Informações sobre como os dados são armazenados.
- Armazenados no **catálogo do SGBD**, que contém:
  - Estrutura de cada arquivo.
  - Tipo e formato de armazenamento de cada tipo de dado.
  - Restrições.

---

## Exemplos de Banco de Dados
- Tabelas relacionadas:
  - **LIVRO**: ID_LIVRO, TÍTULO, ANO, ID_EDITORA.
  - **AUTOR**: ID_AUTOR, NOME, PAÍS.
  - **EDITORA**: ID_EDITORA, NOME, PAÍS.
  - **AUTOR_LIVRO**: ID_AUTOR, ID_LIVRO.

---

## Processamento Tradicional vs Abordagem de BD
- **Processamento Tradicional**:
  - A estrutura dos dados está incorporada ao programa de acesso.
  - Alterações na estrutura de arquivos implicam alterações no código-fonte dos programas.
- **Abordagem de BD**:
  - A aplicação pode manipular diversas bases de dados diferentes.
  - Alterações na estrutura são feitas apenas no catálogo, sem impactar os programas.

---

## Modelo de Dados
- Conjunto de conceitos para descrever a estrutura **conceitual**, **lógica** e **física** de um banco de dados.
- Tipos de Modelos:
  - **Alto nível**: Modelo conceitual, próximo à visão do usuário.
  - **Baixo nível**: Modelo físico, detalha como os dados estão armazenados.

---

## Arquitetura de Três Esquemas
1. **Nível Interno**:
   - Descreve a estrutura de armazenamento físico.
   - Detalhes sobre caminhos de acesso ao banco de dados.
2. **Nível Conceitual**:
   - Descreve a estrutura global do banco de dados.
   - Não fornece detalhes de armazenamento físico.
3. **Nível Externo**:
   - Descreve as visões do banco de dados para grupos de usuários.

---

## Esquema e Instância de um BD
- **Esquema**:
  - Descrição do banco de dados, especificada durante o projeto.
  - Poucas mudanças ocorrem no esquema.
- **Instância**:
  - Dados armazenados em um banco de dados em um determinado instante.
  - Altera-se sempre que há mudanças no banco de dados.

---

## Pessoas Envolvidas em Sistemas de BD
- **Administradores de Bancos de Dados (DBA)**:
  - Responsável pelo gerenciamento lógico e físico do banco de dados.
- **Administrador de Dados (AD)**:
  - Define políticas e padrões de dados.
- **Analista de Dados**:
  - Interpreta dados para tomadas de decisão.
- **Engenheiro de Dados**:
  - Projeta e mantém pipelines de dados.
- **Cientista de Dados**:
  - Aplica técnicas de machine learning e estatística para extrair insights.

---

## Exercícios Propostos
1. **Exercício 01**:
   - Pesquisar e descrever pelo menos 3 SGBDs, incluindo informações sobre licença, fabricante e características.
2. **Exercício 02**:
   - Comparar abordagem tradicional de arquivos vs abordagem de bancos de dados relacionais.
3. **Exercício 03**:
   - Pesquisar e descrever as diferenças entre cargos da área de banco de dados:
     - Administrador de Banco de Dados.
     - Administrador de Dados.
     - Engenheiro de Dados.
     - Projetista de Banco de Dados.
     - Cientista de Dados.

---

## Bibliografia
- ELMASRI, R., NAVATHE, S. *Sistemas de Banco de Dados*. 7ª Edição – São Paulo: Pearson, 2018.
- HEUSER, C.A. *Projeto de Banco de Dados*. 6 ed. Porto Alegre: Bookman, 2009.
- SILBERSHATZ, A. *Sistema de Banco de Dados*. 7. ed. Rio de Janeiro: LTC, 2020.
- DAMAS, L. *SQL - Structured Query Language*. 14 ed. Rio de Janeiro: LTC, 2017.
- MACHADO, F. N. *Banco de Dados - Projeto e Implantação*. 4 ed. São Paulo: Erica, 2020.
- DATE, C. J. *Introdução a Sistemas de Banco de Dados*. 8 ed. Rio de Janeiro: LTC, 2004.
