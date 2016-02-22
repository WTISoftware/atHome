#SB6PRF
####Módulo de pulsadores sem fio

##Manual de operação
O módulo de atuadores é projetado para operar em caixas de parede, ou em locais onde é necessário enviar comandos para qualquer módulo que possa ser integrado com o Sistema wti@home. Leia atentamente as recomendações e instruções de uso. Guarde este Manual de instruções para possíveis consultas.

##ESPECIFICAÇÕES

######Alimentação:
Bateria 3V CR2032
######Comunicação:
Rádio frequência 2.4Ghz, 125 canais adicionais, endereçamento de 24bits
######Protocolo:
@home
######Pulsadores:
6
######Cenas:
6 para “short press”, 6 para “long press”, 10 cenas adicionais
######Umidade:
+5% a 95% não condensado
######Temperatura de operação:
-10°C a +70°C
######Função pânico:
SIM

##INFORMAÇÕES TÉCNICAS

Controlado pelos sistemas wti@home;
Microcontrolado;
O dispositivo pode atuar em qualquer equipamento da linha wti@home

A durabilidade da bateria depende diretamente da quantidade de acionamentos a qual o módulo será submetido e ao tempo de vida útil da própria bateria. Para acionamentos “short press” em intervalos mínimos de 5 segundos, a durabilidade excederá 40.000 acionamentos. Estima-se também que o tempo útil de vida da bateria pode chegar a 2 anos..

O equipamento foi projetado para instalação dentro de caixas 4x2 e 4x4, e somente poderá trabalhar com conectores compatíveis com os procedimentos de segurança.

Evite colocar fios elétricos dentro das mesmas caixas onde o equipamento será instalado pois isso pode causar interferência.

Conexões erradas ou inapropriadas podem ser perigosas.

##1. INFORMAÇÕES GERAIS SOBRE O SISTEMA @HOME
@home é um sistema sem fios, com base na tecnologia de NRFWTI. @home oferece muitas vantagens quando comparado com sistemas similares. Em geral, os sistemas de rádio criam uma conexão direta entre o receptor e transmissor. Entretanto, o sinal de rádio é enfraquecida por uma variedade de obstáculos localizados no seu caminho (paredes do apartamento, mobiliário, etc.) e em casos extremos, incapaz de transferir dados necessários. A vantagem do sistema @home é que os seus dispositivos além de ser transmissores e receptores de sinais, também são “repetidores” de sinal. Quando um caminho de ligação direta entre o transmissor e o receptor pode não ser estabelecido, a ligação pode ser estabelecida através de outros dispositivos intermediários.
@home é um sistema sem fio, ou seja, bidirecional. Isso significa que o sinal não apenas é transmitido para os receptores, mas também os receptores enviam a confirmação da sua recepção. Esta operação confirma seu status de modo a verificar se eles estão ativos.
@home opera na faixa de frequência de 2.4Ghz para transmissão de dados. Cada rede @home tem o seu próprio número de identificação exclusivo (NET ID), além de um canal específico dentro da faixa definida, razão pela qual é possível cooperar dois ou mais sistemas independentes em um único edifício, sem qualquer interferência.
O sistema @home gera uma estrutura de rede dinâmica. Logo após que o sistema @home é ligado, a localização de cada um dos componentes é automaticamente atualizada em tempo real, através de confirmação do estado dos sinais recebidos a partir de dispositivos que operam em rede "mesh".

O módulo de pulsadores @home foi projetado para enviar comandos para equipamentos da linha @home usando ondas de rádio.

##2. INSTALANDO O MÓDULO


######PERIGO DE CHOQUE

1. Antes de ligar o  equipamento verifique que não existem fios elétricos na mesma caixa de parede na qual o módulo pulsador será instalado. Além de provacar interferência, e danos ao produto, fio elétricos podem prejudicar a sua segurança pessoal.

2. Conecte o módulo SB6PRF conforme o diagrama a seguir.

3. O módulo SB6PRF vêm com 2 fios de GND para maior praticidade nas ligações. Não há nenhuma diferença entre eles, podendo ser usado somente um ou ambos indiscrimidamente.

4. Instale o módulo de pulsadores no local determinado.

######NOTAS PARA O DIAGRAMA

P1 – Pulsador 1
P2 – Pulsador 2
P3 – Pulsador 3
P4 – Pulsador 4
P5 – Pulsador 5
P6 – Pulsador 6
GND – Comum para os pulsadores


Módulo de 6 pulsadores

######DICAS PARA AJUSTE DA ANTENA

A antena é localizada na parte interna do equipamento e é sinalizada na etiqueta de identificação do produto. Desta forma, deve-se sempre instalar o equipamento com a etiqueta de identificação voltada para o ambiente a ser controlado.

Superfícies de metal próximas à antena, podem impactar na recepção do sinal.

Reatores ou motores próximos à antena, podem impactar na recepção do sinal.

Lajes de concreto podem impactar na recepção do sinal.

##3. OPERAÇÃO BÁSICA

O módulo SB6PRF é formado por 6 chaves de contato que podem enviar comandos para  para qualquer outro equipamento na rede @home.

Cada uma das 6 chaves de contato P1, P2, P3, P4, P5 ou P6 opera no modo pulsador, que consiste em acionar a chave de contato por um tempo mínimo pré-determinado, para que o cenário correspondente possa ser executado. Neste modo, cada pulsador possui um cenário associado a função “short press”, um cenário associado a função “long press” e um cenário especial chamado “panic”:

1. Acionamento “short press”: Quando o pulsador é acionado por um tempo menor que 500ms.
2. Acionamento “long press”: Quando o pulsador é acionado por um tempo maior que 500ms e menor que 5seg.
3. Botão de “panic”: Quando o pulsador é acionado por um tempo maior que 5seg um comando especial é enviado à central Net Center caso a mesma esteja presente na rede.

As chaves de contato  vem  de fábrica sem nenhuma programação.

Somente é possível alterar a configuração de fábrica através do computador utilizando o adaptador para porta USB que é vendido separadamente.

É necessário alterar o módulo para o “modo de programação”. Vide item 4.

Para utilizar a comunicação com o computador é necessário além do adaptador para porta USB, a instalação do programa de comunicação com portas Seriais. A configuração da porta serial deve ser: 57600, N, 8, 1.

Acesse http://www.wtihome.com.br/suporte para mais informações.

##4. MODO DE PROGRAMAÇÃO

O módulo SB6PRF vem de fábrica configurado no  “modo de economia de energia”.  Este é o modo padrão de operação.

Para alterar qualquer programação do equipamento pela porta de programação é necessário colocar o módulo no “modo de programação”. É importante salientar que este modo gasta 100x mais bateria que no “modo de economia de energia”, devendo o equipamento ficar alimentado por bateria e neste modo o mínimo de tempo necessário. (*)

Para colocar o equipamento no “modo de programação”:

1. Coloque o jumper do adaptador USB para 3.3V. 
2. Coloque o jumper nos pinos ao lado do conector de programação.
3. Insira o adaptador USB no conector de programação.
4. Insira o cabo USB no computador e entre em qualquer programa de emulação de terminal com as configurações descritas anteriormente.
5. Reinicie o equipamento inserindo um objeto de ponta no orifício de reset do equipamento até sentir uma leve pressão.
6. A mensagem “Setup mode enabled”  deve aparecer no programa de emulação de terminal.
 
Para colocar o equipamento no “modo de economia de energia”:

1. Retire o jumper dos pinos ao lado do conector de programação.
2. Reinicie o equipamento inserindo um objeto de ponta no orifício de reset do equipamento até sentir uma leve pressão.

É possível alimentar o módulo somente pelo adaptador USB durante o “modo de programação” visando não consumir a bateria. 
Para isso basta retirar os parafusos laterais do módulo, abrí-lo e retirar a bateria.

A bateria deve ser inserida novamente antes de retornar o módulo para o “modo de economia de energia”. 

Nunca ligue o adaptador USB com o jumper para 5V. Isso pode danificar o equipamento.

##5. COMUNICANDO O EQUIPAMENTO COM OUTROS MÓDULOS

É possível associar vários equipamentos do sistema @home permitindo criar uma rede de equipamentos, cujo principal objetivo é criar cenários complexos e ampliar o alcance da rede. Esta associação pode ser feita mesmo sem a necessidade da central Net Center:

1. Configure cada um dos equipamentos com um endereço diferente mas na mesma (NET ID) para que seja possível que os equipamentos interajam entre si.

2. Posicione os equipamentos de tal forma que nenhum equipamento fique fora do alcance de, pelo menos, um dos equipamentos que se deseja interligar.

3. Altere os cenários pré-determinados para realizar as cenas desejadas.

É possível configurar todas as funções dos equipamentos através do computador e do adaptador USB. 

A central Net Center é necessária quando se deseja controlar os equipamentos através de smartphones ou tablets ou executar cenas em horários pré-determinados.

##6. CENÁRIOS

O módulo SB6PRF pode armazenar até 22 cenários diferentes divididos em 3 bancos chamados: “Banco A”,  “Banco B” e “Banco S”. Os cenários podem ser executados através das chaves de contato.

O banco A, possui 6 posições para cenários chamados A1, A2, A3, A4, A5 e A6. Estes cenários estão diretamente relacionamento com as chaves de contato P1, P2, P3, P4, P5 e P6 respectivamente. Estes cenários são executados quando é acionado o “short press” na respectiva chave de contato. 

O banco B,  possui 6 posições para cenários chamados B1, B2, B3, B4, B5 e B6. Estes cenários estão diretamente relacionados com as chaves de contato P1, P2, P3, P4, P5 e P6 respectivamente. Estes cenários são executados quando é acionado o “long press” na respectiva chave de contato. 

O banco S, possui 10 posições para cenários chamados S0 a S9. Estes cenários não estão associados diretamente as chaves de contato e podem ser executados através do computador e por outros cenários,

Cada cenário pode armazenar um máximo de 24 caracteres. Como um comando básico possui de 3 a 5 caracteres, cada cenário pode armazenar de 5 a 8 comandos. Cada comando deve ser separado pelo caractere “;”. É possível encadear cenários, aumentando consideravelmente a quantidade de comandos executados por vez.

######Exemplo de cenários:

“S0” - Executa o cenário S0
“30:L1” - Envia para o equipamento cujo endereço é 30, o comando “L1”

##7. COMANDOS 

Os seguintes comandos estão disponíveis no módulo SB6PRF podendo ser enviados através das chaves de contato, do conector de programação ou de outros equipamentos, como também da central Net Center.

Se os comandos forem enviados através do conector de programação, ao final de cada grupo de comandos deve ser enviado o caractere LF (Line Feed)

Os comandos seguem o formato:

comando parametro1 parametro2 parametro3 parametro4 onde os parâmetros podem ser opcionais dependendo do tipo de comando.

Para enviar comandos para outros equipamentos, deve-se informar o endereço do equipamento destino, sempre com 2 caracteres, seguido do caractere “:” antes do comando a ser enviado:

######Exemplo:
“30:L1” - Envia para o equipamento cujo endereço é 30, o comando “L1”  

Grupo 1 – Comandos gerais de configuração do rádio e da rede

$RAD – Endereço e outros parâmetros do rádio nRFWTI

######Parâmetros disponíveis:

endereço – Endereço único na rede, no formato hexadecimal (Default: 88 – valores entre 00 e FE). (*)

frequência RF – Variação em 1Mhz da frequência de operação do rádio no intervalo de 2400Mhz a 2525Mhz, seguindo a fórmula: 2400 + Frequencia RF – (Default: 76 – valores entre 0 e 125).

$NET – NET ID e endereço da Central Net Center (*)

######Parâmetros disponíveis:

central – Endereço único da central Net Center, no formato hexadecimal.(Default: FF – valores entre 00 e FF)

offset1 – Primeiro byte do NET ID, no formato hexadecimal (Default: 3C – valores entre 00 e FF) 

offset2 – Segundo byte do NET ID, no formato hexadecimal (Default: 5A – valores entre 00 e FF)

offset3 – Terceiro byte do NET ID, no formato hexadecimal (Default: 69 – valores entre 00 e FF) 

(*) O endereço NET ID é formado por 3 bytes e deve ser igual para todos os equipamentos de uma mesma rede. Mesmo que outra rede esteja na mesma frequência de rádio, o NET ID vai garantir que haja uma independência entre elas. NUNCA DEIXE SEU NET ID COM OS PADRÕES DE FÁBRICA
$PAR – Parâmetros de transmissão do rádio.

######Parâmetros disponíveis:

potência – Potência de transmissão (Default: 3)
0 – Mínima
1 – Média
2 – Alta
3 - Máxima
velocidade – Velocidade de transmissão  (Default: 2)
0 – 1Mbps
1 – 2Mbps
3 – 250Kbps
tamanhoCRC – Quantos bytes ocupa o CRC “Controle de Checagem de Erro” em cada pacote transmitido (Default: 2)
0 – Desabilitado
1 – 8bits
2 – 16bits
$RET – Parâmetros de retransmissão do rádio.

######Parâmetros disponíveis:

atraso – Atraso entre as retransmissões, em múltiplos de 4ms, no caso de falha (Default: 4, valores entre 0 e 15)
quantidade – Quantidade de retransmissões (Default: 4, valores entre 0 e 15)
$NEA – Endereço dos equipamentos próximos. 

Parâmetros disponíveis:

endereço1 a 4 – Endereço de um equipamento próximo , no formato hexadecimal (Default: FF – valores entre 00 e FF) (*)

(*) O endereço FF não é associado a nenhum equipamento e deve ser utilizado quando se deseja retornar ao modo auto-discover: $NEA FF FF FF FF 

######DICAS PARA CONFIGURAÇÃO

A maioria dos comandos de configuração do rádio e da rede já vem pré-definidos de fábrica para seu melhor desempenho. Não é necessário nenhum ajuste adicional.

O endereço do rádio, o NET ID e o canal do rádio por estarem com seus parâmetros default, devem ser alterados para evitar interferência com outros equipamentos ou outras redes. Comandos $RAD e $NET.

Pode-se usar o caractere “?” quando não se deseja alterar o valor de um determinado parâmetro:
Ex: $RAD ? 77 – O endereço do rádio permanece inalterado, e a frequência do rádio foi alterado para o canal 77. 

Grupo 2 – Outros comandos gerais

$SAV – Salva os parâmetros configurados na memória não volátil (EEPROM)
$STA – Envia os parâmetros configurados para a porta de configuração caso o comando tenha sido recebido por ela, ou para o equipamento requisitante.
$SCE – Envia os cenários cadastrados para a porta de configuração.
$FDF – Retorna todos os parâmetros do equipamento para os ajustes de fábrica e executa um reset geral.
$VER – Envia a versão de firmware para a porta de configuração caso o comando tenha sido recebido por ela, ou para o equipamento requisitante.
$RST – Reinicia o equipamento

Grupo 3 – Comandos específicos para o módulo SB6PRF

$DEL – Tempos de configuração do “short press” e do “long press”.

Parâmetros disponíveis:

maximoShortPress – Tempo máximo em ms que uma chave de contato deve ser ativada para que seja considerado como “short press”. (Default: 400ms – Valores entre 1 e 65535 ms)

minimoPanic – Tempo mínimo em ms que uma chave de contato deve ser ativada para que seja considerado como um “panic press”. (Default 4000ms – Valores entre “maximoShortPress” e 65535 ms) (*)

minimoValido – Tempo mínimo em ms que uma chave de contato deva ser ativada para que qualquer tipo de acionamento deva ser considerado. (Default: 25ms – Valores entre 0 e maximoShortPress)

No modo pulsador, o cenário é executado somente após a chave de contato ter sido liberada.

(*) O “long press” é considerado, quando o tempo de acionamento é maior que o maximoShortPress e menor que minimoPanic.

Grupo 4 – Comandos para cenários

A1,A2,A3,A4,A5,A6,B1,B2,B3,B4,B5,B6,S0,S1,S2,S3,S4,S5,S6,S7,S8 e S9 – Executa o cenário. (*)

(*) Os cenários A* e B* também estão associados às chaves de  contato mas funcionam como qualquer outro cenário e podem ser chamados através de outros cenários.
WA1,WA2,WA3,WA4,WA5,WA6,WB1,WB2,WB3,WB4,WB5,WB6,WS0,WS1,WS2,WS3,WS4,WS5,WS6,WS7,WS8,WS9 – Grava o cenário.

######Parâmetros disponíveis:

comandos – Comandos que serão executados pelo cenário específico. Caso seja necessário a execução de mais de um comando, é necessário separar cada comando pelo caractere “;” e o colocar o conjunto inteiro entre aspas duplas:
Ex: 
WA1 “30:L1”
WA2 “S0;S1”
WS0 “30:I1”


##8. PROCEDIMENTOS PARA MAU FUNCIONAMENTO

O equipamento não responde a uma transmissão remota

1. Verifique se o alcance máximo não foi excedido e que o sinal não está obstruído por superfícies ou caixas de metal.

2. Caso o equipamento tenha sido reiniciado recentemente, envie alguns comando adicionais para que a memória dos equipamentos remotos limpe qualquer referência de informação deste equipamento. 


##9. AJUSTES DE FÁBRICA
Caso necessário, é possível ajustar o equipamento para os padrões de fábrica. Entre no “modo de programação” e digite o comando $FDF. 

##10. GARANTIA

######I - PRAZO E COMPROVAÇÃO DA GARANTIA

1. O produto abaixo identificado, devidamente lacrado, é garantido pelo seu fabricante e/ou importador (XSOLUTIONS S.A.), pelo prazo de um ano, contado a partir da data de sua aquisição pelo primeiro consumidor e obedecidas as condições e as recomendações especiais aqui discriminadas.

2. Esta garantia contratual é dada ao produto abaixo identificado, exclusivamente contra eventuais defeitos decorrentes de projeto, fabricação, montagem, ou quaisquer outros vícios de qualidade que o tornem impróprio ou inadequado ao uso regular.

3. Para a comprovação desse prazo, o consumidor deverá apresentar este Termo de Garantia, devidamente preenchido, e/ou a 1ª via da nota fiscal de compra, ou outro documento fiscal equivalente, desde que identifique o produto.
Exija do estabelecimento comercial revendedor, o preenchimento correto deste Termo de Garantia.

######II- EXCLUSÃO DA GARANTIA

A garantia não abrangerá, sendo, pois, ônus do consumidor:

a) Os danos sofridos pelo produto, ou seus acessórios, em consequência de acidente, maus tratos, manuseio ou uso incorreto e inadequado;

b) Os danos sofridos pelo produto, em consequência de sua utilização para finalidades diversas das especificadas pelo fabricante e/ou importador (XSOLUTIONS S.A.), ou incompatíveis com a destinação do mesmo.

######III- LOCAL ONDE A GARANTIA DEVERÁ SER EXERCITADA

1. Os consertos em garantia somente deverão ser efetuados por uma Assistência Autorizada, devidamente nomeada pelo fabricante e/ou importador (XSOLUTIONS S.A.), que, para tanto, se utilizará de técnicos especializados e de peças originais, relacrando o seu aparelho e garantindo o serviço executado.

######IV- CESSAÇÃO DA GARANTIA

1. Não confie o conserto do produto abaixo identificado a curiosos, pessoas ou oficinas não autorizadas e não credenciadas pelo seu fabricante e/ou importador (XSOLUTIONS S.A.).

2. Se isto vier a ocorrer, com a consequente violação do lacre do produto, a garantia cessará, de imediato.

3. O produto abaixo identificado foi projetado para funcionamento em uso doméstico, única e exclusivamente. A sua utilização, para uso não doméstico, industrial ou comercial, acarretará a cessação imediata da garantia.


######V- RECOMENDAÇÕES ESPECIAIS

1. Antes de colocar o produto em funcionamento, leia atentamente as instruções de uso e/ou instalação contidas no próprio aparelho, na embalagem, ou no manual respectivo. Siga-as rigorosamente. Elas são a sua segurança.

2. Certifique-se de que a voltagem a ser utilizada é a mesma indicada no aparelho (110V a 220V). Verifique se a instalação elétrica do local está correta e adquada.

3. Para evitar danos, mantenha o produto bem armazenado e limpo, em ambiente protegido das intempéries (chuva, vento, umidade, raios solares, etc.).

4. Não introduza quaisquer objetos estranhos à função própria do produto, principalmente quando este estiver em funcionamento, evitando acidentes.

######VI - FABRICANTE E/OU IMPORTADOR

XSOLUTIONS S.A. - CNPJ/M.F. Nº 61.064.978/0001-01
Av. Carlos Vasconcelos, 1702 – Aldeota – Fortaleza/CE

Qualquer reclamação, comentário ou sugestão sobre o atendimento e os reparos prestados pelas Assistências Autorizadas, ligue ao nosso Serviço de Atendimento ao Consumidor.


Departamento de Assistência Técnica: (85) 3311.6464
