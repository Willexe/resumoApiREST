# Api REST e RESTful
API REST, ou API RESTful, refere-se a uma interface de programação de aplicações que segue os princípios e restrições do estilo arquitetural REST, que significa "Representational State Transfer" (Transferência de Estado Representacional). Essa abordagem arquitetural foi concebida por Roy Fielding, um cientista da computação. O objetivo da REST é proporcionar uma maneira padronizada e eficiente de comunicação entre sistemas distribuídos na web. As APIs RESTful são fundamentais para a construção de aplicações modernas, permitindo a comunicação eficiente entre diferentes sistemas e plataformas. 
APIs REST utilizam solicitações HTTP para realizar operações padrão de banco de dados (CRUD) em recursos. Exemplos incluem GET para recuperar, POST para criar, PUT para atualizar e DELETE para excluir registros. Todos os métodos HTTP podem ser empregados. Uma API REST bem projetada opera como um site no navegador, integrando funcionalidades HTTP.

## Diferenças entre REST e RESTFUL
- **REST** é uma arquitetura de software que estabelece diretrizes para a comunicação em redes complexas, inicialmente concebida para a internet. Essa abordagem permite uma comunicação confiável e eficiente em grande escala, oferecendo flexibilidade e portabilidade entre plataformas para sistemas de API. APIs que seguem o estilo REST são chamadas de APIs REST, enquanto serviços da Web que implementam essa arquitetura são denominados serviços da Web RESTful. Os termos "API REST" e "API RESTful" são frequentemente usados de forma intercambiável.
- Uma **API RESTful** permite que o cliente solicite recursos ao servidor, seguindo as diretrizes fornecidas na documentação da API. As etapas gerais de uma chamada de API REST incluem o envio de uma solicitação formatada de acordo com a documentação, autenticação e verificação de permissões pelo servidor, processamento interno da solicitação e, finalmente, a resposta do servidor ao cliente, indicando o sucesso da solicitação e fornecendo as informações solicitadas. Os detalhes específicos de solicitação e resposta podem variar conforme a concepção da API pelos desenvolvedores. Em resumo, REST é o conceito geral de um estilo arquitetural, enquanto RESTful se refere à implementação específica de uma API que segue esse estilo, observando suas restrições e princípios.

## HTTP verbs
O protocolo HTTP define métodos de requisição, também conhecidos como HTTP Verbs, que indicam a ação a ser realizada em um recurso. Esses métodos têm semânticas distintas, mas alguns compartilham características como serem safe, idempotentes ou cacheáveis. Safe, idempotente e cacheável são propriedades que podem ser aplicadas a qualquer método de requisição. Esses métodos formam a base para interações HTTP, variando desde solicitações de dados até modificações e exclusões de recursos.
Alguns desses métodos incluem:
1. **GET**:Solicita a representação de um recurso específico, retornando apenas dados.
2. **HEAD**: Semelhante ao GET, mas sem o corpo da resposta.
3. **POST**: Submete uma entidade a um recurso, frequentemente causando mudanças no estado ou efeitos colaterais no servidor.
4. **PUT**: Substitui todas as representações do recurso pelo conteúdo da requisição.
5. **DELETE**: Remove um recurso específico.
6. **CONNECT**: Estabelece um túnel para o servidor identificado pelo recurso.
7. **OPTIONS**: Descreve opções de comunicação com o recurso.
8. **TRACE**: Executa um teste loop-back junto ao caminho para o recurso.
9. **PATCH**: Aplica modificações parciais a um recurso.

Cada método possui semânticas específicas, e alguns compartilham características como serem safe, idempotent ou cacheable. Esses métodos formam a base para interações HTTP, abrangendo desde solicitações de dados até modificações e exclusões de recursos.

## HTTP Status Code
Os códigos de status HTTP são indicadores numéricos retornados por um servidor web em resposta a uma solicitação de um cliente, como um navegador web ou aplicativo. Esses códigos fornecem informações sobre o resultado da solicitação e indicam se a solicitação foi bem-sucedida, foi redirecionada, exigiu ação adicional do cliente ou se ocorreu um erro.
Os códigos de status HTTP são divididos em cinco categorias, cada categoria é representada pelo primeiro dígito do código:

1. **Códigos de informação (1xx):** Indica que a solicitação foi recebida, está sendo processada ou que ações adicionais são necessárias para continuar processando a solicitação.
- **100 Continue:** Indica que o cliente pode continuar com a solicitação. É um sinal para o cliente enviar a próxima parte da solicitação.
- **101 Switching Protocols:** Indica que o servidor está disposto a mudar os protocolos indicados pelo cliente em sua solicitação.
- **102 Processing:** É um código provisório indicando que o servidor recebeu e está processando a solicitação, mas ainda não concluiu ação alguma.
  
2. **Código de sucesso (2xx):** Indica que a solicitação foi bem-sucedida. O servidor entende e aceita ou está processando a solicitação.
- **200 OK:** Indica que a solicitação foi bem-sucedida. A resposta incluirá as informações solicitadas.
- **201 Created:** Indica que a solicitação foi bem-sucedida e resultou na criação de um novo recurso no servidor.
- **204 No Content:** Indica que a solicitação foi bem-sucedida, mas não há conteúdo para ser retornado na resposta.
  
3. **Códigos de redirecionamento (3xx):** Indica que o cliente precisa realizar ações adicionais para concluir a solicitação. Isso geralmente envolve o redirecionamento para outro URL.
- **301 Moved Permanently:** Indica que o recurso solicitado foi permanentemente movido para uma nova localização. O cliente deve redirecionar automaticamente para a nova URL.
- **302 Found:** Indica que o recurso solicitado foi temporariamente movido para uma nova localização. O cliente pode continuar usando a URL original.
- **303 See Other:** Indica que o servidor recomenda uma mudança para outra URI e que a mudança é feita usando o método GET.
  
4. **Códigos de erro do cliente (4xx):** Indica que ocorreu um erro no lado do cliente, como uma solicitação malformada ou acesso não autorizado.
- **400 Bad Request:** Indica que a solicitação feita pelo cliente é inválida, malformada ou contém parâmetros incorretos.
- **401 Unauthorized:** O cliente não está autorizado a acessar o recurso solicitado. Geralmente, isso exige autenticação.
- **403 Forbidden:** Indica que o cliente tem autenticação válida, mas ainda não tem permissão para acessar o recurso solicitado.

5. **Código de erro do servidor (5xx):** indica que o servidor encontrou um erro ao processar a solicitação, geralmente devido a uma falha interna do servidor.
- **500 Internal Server Error:** Indica um erro genérico no servidor que não é mais especificamente abordado por outros códigos de status 5xx.
- **501 Not Implemented:** Indica que o servidor não suporta a funcionalidade necessária para atender à solicitação. Por exemplo, o servidor pode não reconhecer o método de solicitação.
- **502 Bad Gateway:** Indica que o servidor, ao atuar como gateway ou proxy, recebeu uma resposta inválida do servidor upstream.
  
Os códigos de status HTTP são essenciais para a compreensão dos resultados de uma solicitação e são amplamente utilizados no desenvolvimento web para depurar e diagnosticar problemas de comunicação entre clientes e servidores.

**Autor do resumo: William Barbosa de Souza - 01506070**






