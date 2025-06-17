prova1.c
Esse programa lê um arquivo com várias leituras de sensores e separa os dados em vários arquivos, um para cada sensor. Depois, ele organiza as leituras de cada sensor do mais novo para o mais velho
Você roda o programa passando o nome do arquivo que tem os dados (exemplo: ./prova1 leituras.txt).
O programa lê tudo desse arquivo: cada linha tem a hora da leitura (timestamp), o nome do sensor e o valor medido.
Ele guarda todas essas informações na memória.
Depois, para cada leitura, ele cria (ou abre) um arquivo só daquele sensor e salva a leitura lá.
Depois de separar os arquivos, ele identifica todos os sensores diferentes.
Para cada arquivo de sensor, ele lê tudo, organiza as leituras para que as mais recentes fiquem primeiro, e salva de novo o arquivo já arrumadinho.

prova2.c
Esse programa te ajuda a encontrar a leitura de um sensor que está mais perto de uma hora específica que você quer.
Você roda o programa passando o nome do sensor e o horário que quer buscar (exemplo: ./prova2 temp 1650000000).
Ele abre o arquivo desse sensor (tipo "temp.txt") e carrega todas as leituras.
Usa um método rápido para procurar (chamado busca binária) a leitura com a hora mais próxima da que você pediu.
Por fim, ele mostra essa leitura para você.

prova3.c
Esse programa cria um arquivo com várias leituras falsas de sensores, pra você poder testar.
Você fala o intervalo de tempo que quer gerar as leituras (hora inicial e final).
Depois, informa quais sensores quer e o tipo deles, por exemplo: temp,CONJ_Q ou porta,BINARIO.
Para cada sensor, ele cria 2000 leituras dentro desse intervalo de tempo.
O valor de cada leitura muda conforme o tipo do sensor:
CONJ_Z: números inteiros, tipo 0 a 999
CONJ_Q: números com duas casas decimais
BINARIO: "true" ou "false"
TEXTO: palavras aleatórias com letras maiúsculas
Por fim...
Ele salva tudo isso num arquivo chamado leituras.txt.
