# Error/Erro 

Um log de "error" é um tipo de log que deve ser usado quando ocorre um erro que afeta o funcionamento da aplicação, mas que não impede a sua execução. Alguns exemplos de cenários em que pode ser adequado usar um log de "error" incluem:

- Quando ocorre um erro que resulta em uma falha em um processo específico da aplicação, como a falha de uma transação ou a falha de um processo de importação de dados.
- Quando um erro é detectado durante uma operação que pode resultar em problemas de desempenho ou de usabilidade para os usuários.
- Quando um erro é detectado durante uma operação que pode resultar em dados incorretos ou incompletos sendo exibidos aos usuários.
- Quando um erro é detectado durante uma operação que pode resultar em problemas de integridade de dados, como a duplicação de registros ou a perda de dados.

Alguém deve ser alertado para consertar imediatamente, mesmo que seja no meio da noite. Deve haver algum tipo de alerta para eventos de log ERROR no ambiente de produção .

Mas tome cuidado para não usar esse nível de registro muito generosamente porque isso adicionaria muito ruído aos logs e reduziria a importância de um único evento ERROR. 

Você não gostaria de ser acordado no meio da noite devido a algo que poderia ter esperado até a manhã seguinte, não é?