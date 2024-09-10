# Tracing/ Rastreamento

Um nível de log descrevendo eventos mostrando a execução passo a passo do seu código que pode ser ignorado durante a operação padrão, mas pode ser útil durante sessões de depuração estendidas.

Comparado ao DEBUG, é muito fácil definir o que logar no TRACE. Como o nome sugere, queremos registrar todas as informações que nos ajudam a rastrear o processamento de uma solicitação recebida por meio de nosso aplicativo .

Isso inclui:

- Início ou fim de um método, possivelmente incluindo a duração do processamento
- URLs dos endpoints de nosso aplicativo que foram chamados
- Início e fim do processamento de uma solicitação de entrada ou trabalho agendado.
- Quando você está depurando um problema ou um erro na aplicação e precisa de informações ainda mais detalhadas do que os logs de "debug" fornecem.
- Quando você deseja entender o comportamento da aplicação em detalhes extremos.
- Quando você deseja rastrear o fluxo de execução de uma aplicação em nível de linha de código para identificar problemas ou otimizar o desempenho.
- Quando você deseja fornecer informações extremamente detalhadas sobre as operações realizadas pelo código da aplicação.

- É importante notar que os logs de "trace" devem ser usados de maneira apropriada e apenas para fornecer informações extremamente detalhadas sobre o funcionamento interno da aplicação. Em geral, os logs de "trace" são desativados em ambientes de produção, pois podem gerar muitos logs e afetar o desempenho da aplicação. Em caso de dúvida, é sempre recomendável consultar a documentação da aplicação ou o manual de estilo para determinar o nível de log adequado.