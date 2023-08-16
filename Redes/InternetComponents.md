# O que é a internet?

`@Annotation["ISP: Internet Service Provider"]`

## Descrição dos componentes da rede

- Sistemas finais são conectados entre si por enlaces (links) de comunicação e comutadores (switches).

- Eles acessam a Internet por meio de ISPs.

- Os sistemas finais, os comutadores de pacotes e outras peças da internet executam protocolos que controlam o envio e o recebimento de informações.

- O TCP(Trasmission Control Protocol) e o IP(Internet Protocol).

## Descrição de Serviço

`@Annotation["API - Application Program Interface"]`

- Os sistemas finais ligados à Internet oferecem uma Interface de Programação de Aplicação (API).

- A API especifica como o programa solicita à infraestrutura da internet que envie dados a um programa de destino específico.

## Redes de Acesso

- Rede Física que conecta um sistema final ao primeiro roteador de um caminho, partindo de um sistema final até outro qualquer.

## Acesso doméstico: DSL, cabo(HFC), FTTH, Discado, Satélite

- DLS é a linha digital do assinante. É um acesso residencial banda larga que utiliza a infraestrutura de telefone local da operadora.

- O acesso à internet a cabo (HFC)

## Acesso doméstico: DSL

`@Annotation["Up - Envio"]` <br>
`@Annotation["Down - Recebimento"]`

- A linha telefônica conduz, simultaneamente, dados (internet) e sinais telefônicos tradicionais, que são codificados em frequências diferentes.

- Um canal de telefone bidirecional comum, com uma banda de 0 a 4 kHz;
- Um canal upstream (envio de dados) de velocidade média, com uma banda de 4 kHz a 50 kHz;
- Um canal downstream (recebimento de dados) de alta velocidade, com uma banda de 50 kHz a 1 Mhz.

## Acesso doméstico: cabo (HFC)

`@Annotation["CMTS - Sistema de Término do Modem a Cabo"]`

- Neste sistema utiliza-se fibra óptica e cabo coaxial, por isso a rede é denominada híbrida fibra-coaxial (HFC). Um longo caminho de fibra é passado pela rota da rede e vários nós são criados no cabo para prover internet para redes menores.

`@Annotation["ONT: terminal de rede óptico"]` <br>
`@Annotation["OLT terminal de linha óptico"]`

## Acesso doméstico: FTTH

- O conceito FTTH (fiber to the home) é simples - oferece um caminho de fibra óptica da Central Telefônica (CT) diretamente até a residência.

## Acesso discado e enlace de satélite

- Em locais de DSL, HFC e FTTH não disponíveis, podemos contar ainda com o acesso discato ou enlace de satélite.

- O acesso discado por linhas telefônicas tradicionais é baseado no mesmo modelo do DSL, todavia é terrivelmente lento, trabalhando na velocidade de 56 kbps.

- O enlace de satélite pode ser empregado para conexão em velocidades desde 1 Mbit/s até as disponibilizadas por cada provedor. Exemplo de provedores de acesso por satélite: StarBand e HughesNet.

## Meios Físicos

- O bit, ao viajar da origem ao destino, passa por uma série de pares transmissor-receptor, que o recebem por meio de ondas eletromagnéticas ou pulsos ópticos que se propagam por um meio físico.

- Alguns exemplos de meios físicos são: par-trançado, cabo coaxial, cabo de fibra óptica, espectro de rádio terrestre e espectro de rádio por satélite.

- Os meios físicos se enquadram em duas categorias: meios guiados e meios não guiados.

## O núcleo da rede

Após termos examinado a periferia da Internet, vamos agora nos aprofundar mais no núcleo da rede - a rede de comutadores de pacote e enlaces que interconectam os sistemas finais da Internet.

## Comutação de Pacotes

- Através de uma aplicação de rede, sistemas finais trocam mensagens entre si.

- Para enviar uma mensagem de um sistema final de origem para um sistema final de destino, o originador fragmenta mensagens em porções de dados menores, denominados pacotes.

- Entre origem e destino.

## Comutação de Pacotes: Transmissão armazena-e-reenvia

- Significa que o comutador de pacotes deve receber o pacote inteiro antes de poder começar a transmitir o primeiro bit para o enlace de saída.

## Comutação de Pacotes: Tabelas de repasse e protocolos de roteamento

- Cada roteador possui uma tabela de repasse que mapeia os endereços de destino para enlaces de saída desse roteador.

- O processo de roteamento fim a fim é semelhante a um motorista que não quer consultar o mapa, preferindo pedir informações.

- Um protocolo de roteamento pode, por exemplo, determinar a distância mais curta entre a máquina de origem e a máquina de destino.

### Tabela de repasse local 
| endereço destino | link de saída |
|-----------|----------|
| faixa-endereços 1 | 3 |
| faixa-endereços 2 | 2 |
| faixa-endereços 3 | 2 |
| faixa-endereços 4 | 1 |

<br>

## Comutação de Circuitos

- As redes de telefonia tradicionais são exemplos de redes de comutação de circuitos. Nessas redes, os recursos necessários ao longo do caminho (buffers, taxa de transmissão de enlaces) para oferecer comunicação entre os sistemas finais, são reservados pelo período da sessão de comunicação entre os sistemas finais.

## Multiplexação em Redes de Comutação de Circuitos

- Um circuito é implementado em um enlace por multiplexação por divisão de frequência.

- Com FDM, cada circuito dispõe continuamente de uma fração da largura da banda.

- Com TDM, cada circuito dispõe de toda a largura de banda periodicamente, durante breves intervalos de tempo.

## Vazão nas Redes de Computadores

- Para definir a vazão, considere a transferência de um arquivo grande do hospedeiro A para o hospedeiro B por uma rede de computadores.

- A vazão instantânea é a taxa (em bits/s) em que o hospedeiro B está recebendo o arquivo.

- Se o arquivo consistir em F bits e a transferência levar T segundos para o hospedeiro B receber todos os F bits, então a vazão média de transferência do arquivo é F/T bits/s.

## Alguns componentes da internet

- Host
- Servidor
- Movel
- Roteador
- Switch
- Model
- Estação Base
- Smartphone
- Torre de Telefonia Celular
