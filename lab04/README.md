# Serviços
*Lab de Componentização e Reúso de Software 22/08/2020*

No link do Google Drive [modelo](https://docs.google.com/presentation/d/1ujoME3qoriVm7hHiC8uK2qWQ3mmHA81Qxe8n80vZYms/edit?usp=sharing) ou no diretório [resources/](resources/) você encontrará um modelo para resolver duas tarefas:

Para as Tarefas 1, 2 e 3 que estão listadas dentro dos slides:

## Tarefa 1
*Componentes de Negócio*

Delimite partes do diagrama à esquerda que você avalia que deveriam estar dentro de um componente.

## Tarefa 2
*Componentes Técnicos*

Separe os componentes do View daqueles definidos no Controller.

## Tarefa 3
*Componentes Técnicos*

Separe os componentes do Model daqueles definidos no Controller.

## Tarefa 4

Encontre dois serviços REST interessantes, que recebam no mínimo dois parâmetros e execute pelo menos uma consulta em cada um deles. Apresente para cada serviço que você escolheu:
* o título do serviço
* a URI do serviço
* uma breve descrição do mesmo
* o cabeçalho HTTP da requisição
* o cabeçalho e conteúdo JSON, XML ou outro formato da resposta

### Sevico: Poemas.
* Titulo poemist
* URL: https://www.poemist.com/api/v1/randompoems
* Descricao: Uma API que retorna Poemas aleatoriamente.
* Metodo: GET
* Cabecalho Request:
~~~ http
Accept: text/html,application/xhtml+xml,application/xml;q=0.9,image/avif,image/webp,image/apng,*/*;q=0.8,application/signed-exchange;v=b3;q=0.9
Accept-Encoding: gzip, deflate, br
Accept-Language: pt-BR,pt;q=0.9,en-US;q=0.8,en;q=0.7
Cache-Control: max-age=0
Connection: keep-alive
Host: www.poemist.com
Sec-Fetch-Dest: document
Sec-Fetch-Mode: navigate
Sec-Fetch-Site: none
Sec-Fetch-User: ?1
Upgrade-Insecure-Requests: 1
User-Agent: Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_6) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/85.0.4183.83 Safari/537.36
~~~
* Cabecalho Resposta:
~~~ http
HTTP/1.1 200 OK
Date: Sat, 29 Aug 2020 02:31:54 GMT
Server: Apache
Upgrade: h2
Connection: Upgrade, Keep-Alive
Cache-Control: no-cache, private, max-age=172800
X-RateLimit-Limit: 20
X-RateLimit-Remaining: 18
Expires: Mon, 31 Aug 2020 02:31:54 GMT
Content-Length: 7803
Keep-Alive: timeout=5, max=100
Content-Type: application/json
~~~
* Body Resposta:
~~~ json
[
    {
        "title": "Dear Jesus",
        "content": "You brought the morning that shines\nClear pearly drops of dew so fine\nYou honey dew the flowers kissed\nBright rosebud born among the mist\nAt your command day turned to night\nThousand stars shined with silvery light\nBusy bees began their flight\nYou hung luscious grapes upon the vine\nOut of water you made wine\nYou are master of the rain\nWith love heal people who are in pain\nUpon troubled waters you walked with grace\nWith calm and peace upon your face\nYou fed a thousand hungry souls\nWith two fish and seven loaves\nYou made cheerful birds that sing\nColorful rainbows refreshing rain\nOn the fence sweet climbing roses\nFresh delicate fragrant posies\nDear Jesus just one more thing\nfrom my heart that I must say\nThank you for this beautiful day",
        "url": "https://www.poemist.com/bobby-marbles-mobley/dear-jesus",
        "poet": {
            "name": "Bobby Marbles Mobley",
            "url": "https://www.poemist.com/bobby-marbles-mobley"
        }
    },
    {
        "title": "Distant View Of England From The Sea",
        "content": "Yes! from mine eyes the tears unbidden start,\nAs thee, my country, and the long-lost sight\nOf thy own cliffs, that lift their summits white\nAbove the wave, once more my beating heart\nWith eager hope and filial transport hails!\nScenes of my youth, reviving gales ye bring,\nAs when erewhile the tuneful morn of spring\nJoyous awoke amidst your hawthorn vales,\nAnd filled with fragrance every village lane:\nFled are those hours, and all the joys they gave!\nYet still I gaze, and count each rising wave\nThat bears me nearer to my home again;\nIf haply, 'mid those woods and vales so fair,\nStranger to Peace, I yet may meet her there.",
        "url": "https://www.poemist.com/william-lisle-bowles/distant-view-of-england-from-the-sea",
        "poet": {
            "name": "William Lisle Bowles",
            "url": "https://www.poemist.com/william-lisle-bowles"
        }
    },
    {
        "title": "Night Lily '19",
        "content": "Appearing nightly on a hard wood floor\r\nPacing, pacing, and pacing\r\nSometimes forgetting what sleep is for\r\nMy worrysome mind is racing\r\n\r\n( chorus )\r\nShe bloomed like a lily at night\r\nThen she faded by the morning light\r\n\r\n\r\nDaydreaming after I sit down\r\nWatching colors run\r\nThen the heart ache comes around\r\nBlinded by the morning sun\r\n\r\n( chorus )\r\nShe bloomed like a lily at night\r\nThen she faded by the morning light\r\n\r\n( bridge )\r\nA fertile soil where only weeds grow\r\nWhen once their was a bouquet\r\nThe barren winter\r\nWhere stems will splinter\r\nTo the harsh light of day\r\nNow I have nothing to show\r\n\r\n( chorus )\r\nShe bloomed like a lily at night\r\nThen she faded by the morning light",
        "url": "https://www.poemist.com/john-hanover/night-lily-19",
        "poet": {
            "name": "John Hanover",
            "url": "https://www.poemist.com/john-hanover"
        }
    },
    {
        "title": "The Deficiency Child",
        "content": "It saddens my heart to see you,\n Little child of woe.\n So early in life, you suffered pain\n And the scars there still remain.\n\n What hope lies for you?\n Is there something I can do?\n I'll try.\n Don't you give up hope.\n Fight on, little child of woe.\n\n We can all make a difference!\n 1. We can support the worldwide project.\n 2. We can help others understand.\n 3. Make a personal contribution.\n 4. Join the Kiwanis mission to virtually eliminate iodine\n deficiency around the world by the year 2000.\n 5. Learn more about Iodine Deficiency Disorder.\n\n Teach me to feel another's woe.\n to hide the fault I see.\n That mercy I to others show.\n That mercy show to me.",
        "url": "https://www.poemist.com/vaudaline-thomas/the-deficiency-child",
        "poet": {
            "name": " Vaudaline Thomas",
            "url": "https://www.poemist.com/vaudaline-thomas"
        }
    },
    {
        "title": "In The Valley Of Cauteretz",
        "content": "All along the valley, stream that flashest white,\n    Deepening thy voice with the deepening of the night,\n    All along the valley, where thy waters flow,\n    I walk'd with one I loved two and thirty years ago.\n    All along the valley, while I walk'd to-day,\n    The two and thirty years were a mist that rolls away;\n    For all along the valley, down thy rocky bed,\n    Thy living voice to me was as the voice of the dead,\n    And all along the valley, by rock and cave and tree,\n  The voice of the dead was a living voice to me.",
        "url": "https://www.poemist.com/alfred-lord-tennyson/in-the-valley-of-cauteretz",
        "poet": {
            "name": "Alfred Lord Tennyson",
            "url": "https://www.poemist.com/alfred-lord-tennyson"
        }
    }
]
~~~

### Servico: Localizacao da IIS
* Nome: Servicao de informacoes da IIS (Estacao Espacial)
* URI: http://api.open-notify.org/iss-now.json
* Descricao: Este endpoint traz as informacoes sobre a atual localizacao da IIS em latitude e longitude.
* Cabecalho da request:
~~~ http
GET /iss-now.json HTTP/1.1
Host: api.open-notify.org
Connection: keep-alive
Upgrade-Insecure-Requests: 1
User-Agent: Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_6) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/85.0.4183.83 Safari/537.36
Accept: text/html,application/xhtml+xml,application/xml;q=0.9,image/avif,image/webp,image/apng,*/*;q=0.8,application/signed-exchange;v=b3;q=0.9
Accept-Encoding: gzip, deflate
Accept-Language: pt-BR,pt;q=0.9,en-US;q=0.8,en;q=0.7
~~~
* Cabecalho da Resposta:
~~~ http
Server: nginx/1.10.3
Date: Sat, 29 Aug 2020 02:45:59 GMT
Content-Type: application/json
Content-Length: 112
Connection: keep-alive
access-control-allow-origin: *
~~~
* Body da Resposta:
~~~ json
{
    "timestamp": 1598669004,
    "iss_position": {
        "longitude": "29.1493",
        "latitude": "47.6193"
    },
    "message": "success"
}
~~~