# wiremock-simple-example
Simple example using wiremock

# Executando wiremock
	java -jar wiremock-standalone-2.8.0.jar --port 8085 --global-response-templating

# URLs válidas
| URL | Mapeamento |
| --- | --- |
| /alguma/url | Body com o texto "Alguma url foi chamada com sucesso!!!" |
| /alguma/url2 | Json mapeado no arquivo result1.json |
| /algum/erro | Erro com status code 404 |
| /alguma/url3/{qualquer_parametro} | Json mapeado no arquivo result2.json onde o valor para campo1 = {qualquer_parametro} |

Post detalhado sobre esse exemplo pode ser encontrado em http://www.reyoko.com/blogui/
