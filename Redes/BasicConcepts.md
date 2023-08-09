# Conceitos Básicos de Redes de Computadores

### Formatos para organização de uma rede (Topologia)

Uma rede de computadores pode ser organizada de diferentes formas, dependendo da quantidade de máquinas, algumas formas se tornam mais ou menos eficientes para transmitir dados pela rede. Dentre eles estão:

- Topologia Estrela: É organizado com os dispositivos dependentes em torno de um dispositivo central que conecta os dependentes de forma indireta (passando pelo dispositivo central).

- Topologia Barramento: Os dispositivos são conectados a um único cabo compartilhado, pode ter problemas de desempenho a medida que mais dispositivos são adicionados, pois se pode ter 1 dispositivo enviando ou recebendo dados por vez.

- Topologia Anel: Os dispositivos são ligados conforme a topologia barramento, com a diferença que o ultimo dispositivo estará conectado ao primeiro, fechando assim um anel. Os dados serão sempre transmitidos em sentido horário.


### Transmissão de dados

- Os dados da rede não são transmitidos inteiramente, são realizadas partições do arquivo em partes menores, os chamados Pacotes (packages), e estes por sua vez, são divididos em Quadros (frames).
Utilizando os frames, os transmissores de sinal irão usar impulsos elétricos (binário) para transmitir os dados via sinal.

### Protocolos

Os protocolos são conjuntos de regras que definem o formato e significados dos quadros.

### Modelos de referência

- 1 - Model `OSI`: O modelo OSI define um conjunto de camadas para o gerenciamento da rede, será descrito posteriormente.

### Camadas do Modelo de Referência OSI (Open Systems Interconnection)

<br>
<br>

Padronização devenvolvida pela ISO (International Standard Organization)

O modelo OSI em si não é uma arquitetura de rede, pois não especifica os serviços e os protocolos exatos que devem ser usados em cada camada. `Ele apenas informa o que cada camada deve fazer`.

## Camadas de transmissão

- Camada 7: Aplicação -> Contém uma série de protocolos necessários para os usuários. Um protocolo amplamente utilizado é o HTTP (Hyper Text Transfer Protocol), que constitui a base para a (WWW) World Wide Web. Quando um navegador deseja uma página da Web, ele envia o nome da página desejada ao servidor, utilizando HTTP. Então o servidor transmite o site de volta.

- Camada 6 - Camada de Apresentação -> É o início da conversão das informações na tela para a linguagem de máquina, seja por compressão ou por criptografia.

- Camada 5 - Camada de Sessão -> A camada de sessão permite que duas aplicações em coputadores diferentes estabeleçam uma sessão de comunicação. Caso o arquivo dê algum problema de transmissão, os computadores reiniciam a trandferência a partir do ponto em que ocorreu essa falha.

- Camada 4 - Camada de Transporte -> É responsavel por pegar os dados enviados pela camada de sessão e quebrar em pacotes. Após isso, os pacotes são colocados em ordem para envio. A máquina receptora remonta os pacotes e se estiverem fora de ordem, ela as coloca em ordem novamente antes de enviá-los a caada de sessão.

- Camada 3 - Camada de Rede -> É responsavel pelo endereçamento, convertendo os enredeços lógicos (IP) em endereços físicos (Endereço MAC). Determina a rota para atingir o destino, baseada em fatores como condições de tráfego da rede e prioridade. O controle de congestionamento e a qualidade do serviço fornecido (retardo, tempo em trânsito, etc.) também são questões da camada de rede.