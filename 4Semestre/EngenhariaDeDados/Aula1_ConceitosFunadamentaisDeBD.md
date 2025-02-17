# Modelo Conceitual de Banco de Dados

## Introdução ao Modelo Entidade-Relacionamento
- **Proposto por Peter Chen**, baseado no princípio: "O mundo está cheio de coisas que possuem características próprias e que se relacionam umas com as outras."
- Utilizado para representar situações do mundo real, identificando objetos (entidades), suas características (atributos) e associações (relacionamentos).

---

## Minimundo
- Descrição de uma parcela do mundo real usada para construção de modelos e diagramas.
- Elementos importantes:
  - Contextualização do problema.
  - Necessidades a serem atendidas.
  - O que precisa ser armazenado:
    - Entidades.
    - Atributos.
    - Relacionamentos.
    - Regras de Negócio.

---

## Entidades
- Conjunto de objetos com os mesmos tipos de características.
- Exemplos: Máquina, Funcionário, Animal.
- Representação gráfica inclui nome da entidade e instâncias.

### Identificação de Entidades
- Coisas tangíveis (Meio de Transporte, Animal, Equipamento).
- Funções exercidas por elementos (Especialista, Cliente, Atendente).
- Eventos ou ocorrências (Vôo comercial, Acidente de trânsito).
- Interações (Compra de imóvel, Venda realizada por um fornecedor).
- Especificações (Modelo de refrigerador).

---

## Atributos
- Características comuns a todas as instâncias de uma entidade.
- Tipos de atributos:
  - Simples ou Atômicos vs Compostos.
  - Monovalorados vs Multivalorados.
  - Armazenados vs Derivados.
  - Chave ou Atributo Identificador vs Não-Chave.

---

## Relacionamentos
- Associações entre instâncias de entidades.
- Pode ser binário, ternário ou n-ário.
- Incluem multiplicidade (participação + cardinalidade) e papéis para especificar funções em relacionamentos.

---

## Entidades Fracas
- Dependem de outras entidades para identificação.
- Possuem chave parcial e participam totalmente nos relacionamentos de identificação.

---

## Especialização e Generalização
- **Especialização**: Processo top-down de identificar subclasses mais especializadas.
- **Generalização**: Processo bottom-up de definir superclasses genéricas a partir de entidades especializadas.
- Restrições de completude e exclusividade ajudam a definir como subclasses interagem com a superclasse.

---

## Mapeamento para Modelo Lógico
- Entidades geralmente viram tabelas.
- Atributos compostos e multivalorados podem exigir tabelas adicionais.
- Relacionamentos são mapeados conforme sua multiplicidade (1:N, 1:1, M:N).
- Três maneiras principais de mapear hierarquias de especialização/generalização:
  1. Uma relação para toda a hierarquia.
  2. Uma relação por entidade especializada.
  3. Uma relação por entidade (preferida por melhor representar o modelo).

---

## Autorrelacionamento
- Quando uma entidade se relaciona consigo mesma.
- Útil para evitar duplicação no modelo.

---

## Notações
- Comparação entre notações de Peter Chen e James Martin ("pés-de-galinha").

---

## Exercícios Práticos
1. **Exercício 01**: Criar um minimundo (tema livre) utilizando os conceitos abordados.
2. **Exercício 02**: Modelar entidades e classificar atributos para o minimundo "Empresa".
3. **Exercício 03**: Utilizar o BR Modelo para modelar as entidades encontradas no exercício 02.
4. **Exercício 04**: Elaborar o DER do minimundo "Empresa".
5. **Exercício 05**: Criar um modelo conceitual com entidade fraca (domínio de sócio de clube).
6. **Exercício 06**: Criar um modelo conceitual com entidade fraca (turmas de disciplina).
7. **Exercício 07**: Criar um DER para gerenciamento de atendimento em TI.
8. **Exercício 08**: Criar um DER para registro policial.
9. **Exercício 09-16**: Mapear modelos conceituais para lógicos, considerando diferentes cenários.

---

## Bibliografia
- HEUSER, C.A. *Projeto de Banco de Dados*.
- ELMASRI, R., NAVATHE, S. *Sistemas de Banco de Dados*.
- SILBERSHATZ, A. *Sistema de Banco de Dados*.
- DAMAS, L. *SQL - Structured Query Language*.
- MACHADO, F. N. *Banco de Dados - Projeto e Implantação*.
- DATE, C. J. *Introdução a Sistemas de Banco de Dados*.
