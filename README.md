newman run minha_colecao.postman_collection.json -e workspace.postman_globals.json

Como guia, há uma referência a alguns códigos básicos de Newman para execução:

Execute apenas uma coleção. Isso pode ser usado se não houver dependência de arquivo de dados de teste ou ambiente.
newman run <nome da coleção>

Execute uma coleção e um ambiente. O indicador -e é para ambiente.
newman run <nome da coleção> -e <nome do ambiente>

Execute uma coleção com o número desejado de iterações.
newman run <nome da coleção> -n <nº de iterações>

Executar com arquivo de dados.
newman run <nome da coleção> --data <nome do arquivo> -n <nº de iterações> -e <nome do ambiente>

Defina o tempo de atraso. Isso é importante, pois os testes podem falhar se forem executados sem atraso, devido a solicitações iniciadas sem que a solicitação anterior conclua o processamento no servidor de terminal.
newman run <nome da coleção> -d <tempo de atraso>


https://api.predic8.de/shop/docs#/

https://api.predic8.de/shop