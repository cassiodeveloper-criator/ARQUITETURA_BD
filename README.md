# Arquitetura de Banco de Dados (BD)

Arquitetura é a forma como os dados são organizados, estruturados e armazenados em um sistema.

Ela define três pilares fundamentais:
- Como salvar dados de forma eficiente e segura  
- Como buscar informações rapidamente  
- Como relacionar diferentes conjuntos de dados  

A escolha da arquitetura impacta diretamente a **performance**, **segurança** e **escalabilidade** da aplicação.

---

# Banco Relacional

Modelo em que os dados são organizados em **tabelas** que se relacionam entre si, formando uma estrutura lógica.

Cada tabela representa uma entidade específica (ex: ALUNOS, PRODUTOS) e os relacionamentos conectam diferentes informações.

### Uso comum:
- Sistemas escolares e universitários  
- Bancos e instituições financeiras  
- Registros médicos e hospitais  

---

# Estrutura das Tabelas

Uma tabela organiza dados em duas dimensões:

## Linhas (Tuplas)
Cada linha representa um registro único.  
Ex: Um aluno específico, um produto.

## Colunas (Atributos)
Cada coluna representa um tipo de informação.  
Ex: Nome, CPF, Turma.

### Exemplo — Tabela Alunos

ID | Nome  | Turma  
1  | João  | 2° DS  
2  | Maria | 2° TI  

---

# Chave Primária (ID)

Cada registro possui um identificador único.

🏹 **Por que usar?**
- Evita duplicação  
- Garante que cada item seja único no sistema  

---

# Relacionamentos entre Tabelas

As tabelas podem se conectar para representar relações do mundo real.

### Exemplo:

Alunos: ID, Nome, Turma  
Matrículas: ID_Aluno, ID_Disciplina, Ano  
Disciplinas: ID, Nome, Professor  

### Relacionamento:

Um aluno pode estar matriculado em várias disciplinas.  
Uma disciplina pode ter vários alunos.

### Benefício:

- Evita repetição de dados  
- Mantém a integridade do sistema  
