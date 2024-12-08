# Pacote PKG_ALUNO

## Descrição
O pacote `PKG_ALUNO` contém um conjunto de procedures e cursores que implementam operações relacionadas à entidade Aluno. Este pacote permite a exclusão de alunos, listagem de alunos maiores de 18 anos e filtragem de alunos por curso.

## Procedures e Cursores

### Procedure de Exclusão de Aluno
**Nome:** `EXCLUIR_ALUNO`

**Descrição:** 
Exclui um aluno da tabela de alunos e remove todas as matrículas associadas a ele.

**Parâmetros:**
- `P_ID_ALUNO` (NUMBER): ID do aluno a ser excluído.

**Exemplo de Uso:**
```sql
BEGIN
  PKG_ALUNO.EXCLUIR_ALUNO(1);
END;
/
