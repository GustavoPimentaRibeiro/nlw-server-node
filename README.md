# server-node

Projeto criado através do evento NLW Node da Rocketseat

# pass.in

O pass.in é uma aplicação de **gestão de participantes em eventos presenciais**.

A ferramenta permite que o organizador cadastre um evento e abra uma página pública de inscrição.

Os participantes inscritos podem emitir uma credencial para check-in no dia do evento.

O sistema fará um scan da credencial do participante para permitir a entrada no evento.

## Requisitos

### Requisitos funcionais

- [ ] O organizador deve poder cadastrar um novo evento;
- [ ] O organizador deve poder visualizar dados de um evento
- [ ] O organizador deve poder visualizar a lista de participantes
- [ ] O participante deve poder se inscrever em um evento;
- [ ] O participante deve poder visualizar seu crachá de inscrição;
- [ ] O participante deve poder realizar check-in no evento;

### Regras de negócio

- [ ] O participante só pode se inscrever em um evento uma única vez;
- [ ] O participante só pode se inscrever em eventos com vagas disponíveis;
- [ ] O participante só pode realizar check-in em um evento uma única vez;

### Requisitos não-funcionais

- [ ] O check-in no evento será realizado através de um QRCode;

### Anotações

Métodos HTTP: GET, POST, PUT, DELETE, PATCH, HEAD, OPTIONS...
Corpo da requisição: Request Body
Parâmetros de busca: Query Params / Search Params -> Para filtros `http://localhost:3333/users?name=Gustavo`
Parâmetros de rota: Route Params -> Identificação de recursos `http://localhost:3333/users/1`
Cabeçalhos: Headers -> Contextos (Cookies, Authorization, Timezone, etc)

20x => Sucesso
30x => Redirecionamento
40x => Erro do cliente (erro em alguma informação enviada por QUEM está fazendo a chamada p/ API)
50x => Erro do servidor (um erro que está acontecendo INDEPENDENTE do que está sendo enviado p/ o servidor)
