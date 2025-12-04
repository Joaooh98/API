# API, REST e RESTFULL.

## API (Application Programming Interface) Interface de Programação de Aplicação


    Cliente (client)
    Garçon (pedidos, levar pedidos para cozinha) (API)
    Cozinha (server)

    Basicamente um conjunto de rotinas e padroẽs estabelecidos por uma aplicação, para que outras aplicaçoes possam utilizar as funcionalidades desta aplicação.

    - Responsavel por estabelecer comunicação entre diferentes serviços 
    - Meio de campo entre as tecnologias.
    - Intermediador para troca de informações.

## REST
 
    Transferencia de estado Representativo, a tranferencia de dados, geralmente, e feita usando o protocolo HTTP.

    O Rest, delimita algumas obrigaçoes nessas tranferencias de dados.

    Resources sera então, uma entidade, um objeto.

### 6 Necessidade (constraints para ser RESTful)

    -_Cliente-servidor_: Separação do cliente e do armazenamento de dados (servidor), dessa forma, poderemos ter uma portabilidade do nosso sistema, usando o React para WEB e React Native para o smartphone, por exemplo. 

    -_Stateless_: Cada requisição que o cliente faz para o servidor, devera conter todas as informaçoẽs necessárias para o servidor entender e responder (RESPONSE) a requisição (REQUEST).
    
    Exemplo: a sessão do usuario devera ser enviada em todas as requisições, para saber se aquele usuario está autenticado e apto a usar os serviços, e o servidor não pode lembrar que o cliente foi autenticado na requisição anterior. Nos nossos cursos, temos por padrão usar tokens para as comunicações. 

    -_Cacheable_: As respostas para uma requisição, deverão ser explicitas ao dizer se aquela requisição, pode ou não ser cachada pelo cliente.

    -_Layered System_: O cliente acessa a um endpoit, sem precissar saber de complexidade, de quais passos estão sendo necessarios para o servidor responder a requisição, ou quais outras camadas o servidor estará lidando, para que a requisição eja respondida. 

    -_Code on demand(opcional)_: Possibilita a nossa aplicação pegar codigos, como o java, e executar no cliente 

## RESTful

    RESTFULL, é a aplicação dos padroes REST. 

## BOAS PRATICAS 

    - Utilizar verbos HTTP para nossas requisiçoes.
    - Utilizar plural ou singular na criação dos endpoits? _NÃO IMPORTA!_ use um padrão!!
    - Não deixar barra na final do endpoint
    - nunca deixar o cliente sem responsta.

## VERBOS HTTP

    - GET: receber dados de uma Resource.
    - POST: Enviar dados ou informações para serem processados por um Resource.
    - PUT: Atualiza dados da Resurce.
    - DELETE: Deletar um Resurce.

## STATUS DAS RESPOSTA HTTP

    CONSULTAR NESSE SITE OS STATUS DAS RESPOSTAS 
    https://developer.mozilla.org/pt-BR/docs/Web/HTTP/Status
