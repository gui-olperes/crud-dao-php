# 1. No contexto da programação orientada a objetos, explique o que é uma "interface".
- É um conjunto de métodos (funções) que uma classe deve implementar para poder ser considerada compatível com a interface. Uma interface define apenas a assinatura 
- dos métodos, ou seja, o nome dos métodos, os parâmetros que eles recebem e o tipo de retorno que eles produzem. Ela não contém a implementação real dos métodos, apenas 
- sua definição.

# 2. O que são "traits" no PHP?
- São uma forma de reutilizar código entre classes sem a necessidade de herança múltipla. Com traits, é possível definir um conjunto de métodos que podem ser usados em 
- diversas classes independentes, possibilitando a criação de uma composição de comportamentos. Em termos simples, um trait é uma coleção de métodos que pode ser 
- incluída em uma classe usando a palavra-chave use. Os métodos do trait se tornam disponíveis para a classe que o utiliza, e são executados como se fossem definidos 
- diretamente na classe.

# 3.Qual(is) a(s) diferença(s) entre os métodos "bindParam" e "bindValue"?
- Tanto bindParam quanto bindValue são métodos utilizados para vincular valores a parâmetros de uma consulta preparada (prepared statement) em bancos de dados. A 
- principal diferença entre os dois métodos é a forma como o valor é vinculado ao parâmetro. O método bindParam vincula o parâmetro a uma referência de variável, 
- enquanto o método bindValue vincula diretamente o valor ao parâmetro. Isso significa que, se você usar bindParam para vincular uma variável a um parâmetro, qualquer
- mudança na variável afetará o valor do parâmetro na consulta preparada. Já com bindValue, o valor vinculado não será afetado pelas alterações na variável. Além disso, 
- o método bindParam permite vincular parâmetros de saída, que são usados para retornar valores após a execução da consulta preparada. O método bindValue não permite
- essa funcionalidade. Em resumo, bindParam é usado quando você deseja vincular um parâmetro a uma variável e quando precisa de parâmetros de saída. Já bindValue é usado 
- quando você deseja vincular diretamente um valor ao parâmetro, sem precisar de uma variável intermediária e sem a necessidade de parâmetros de saída.