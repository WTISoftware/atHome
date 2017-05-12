# B3R3PRF

#### Módulo de 3 relés e 3 pulsadoress

## Manual de operação  
O módulo de atuadores é projetado para operar em locais onde o controle de um dispositivo elétrico (até 1kW) é necessário, tais como forros, lajes, etc. É igualmente possível enviar um sinal para qualquer módulo que possa ser integrado com o Sistema **@home**. Leia atentamente as recomendações e instruções de uso.

## Especificações
Item | Descrição 
------------ | -------------
**Alimentação** | 110/220v
**Consumo nominal** | 4ma
**Comunicação** | Rádio frequência 2.4Ghz, 127 canais adicionais, endereçamento de 24bits
**Protocolo** | @home
**Atuadores** | 3 relés com capacidade de 5A/220v ou 10A/110v
**Chaves de contato** | 3
**Cenas** | 3 para _**“short press”**_, 3 para _**“long press”**_, 10 cenas adicionais
**Umidade** | +5% a 95% não condensado
**Temperatura de operação** |-10°C a +70°C
**Função pânico** | SIM

## Informações Técnicas 

 * Controlado pelos sistemas *@home*  
 * Microcontrolado  
 * Tipo de acionamento: **relés**  
 * O dispositivo pode ser operado remotamente ou por pulsadores e interruptores convencionais  

<img src="/imagens/perigo.de.choque.png" height="40" witdh="40"> Perigo de choque elétrico !
------------
 * Todos os trabalhos no dispositivo só podem ser executados por um eletricista ou pessoa qualificada. Observe os regulamentos nacionais.
 * Mesmo quando o dispositivo está desligado, a tensão pode estar presente nos seus terminais. Qualquer obra que introduza alterações nas configurações de conexões ou à carga, deve ser sempre realizada com a rede elétrica desligada.

<img src="/imagens/i.png" height="40" witdh="40">  Informações
------------
  * A durabilidade do equipamento depende diretamente da carga aplicada. Para cargas resistivas (ex. Lâmpadas incandescentes, etc) e corrente de 5A  em 220V e 10A em 110V, a durabilidade excederá 100.000 acionamentos.  Para cargas indutivas (ex. Lâmpadas Fluorescentes, etc), com cos = 0,6, a corrente de fluxo deve ser limitada a 75% da carga resistiva, para garantir a confiabilidade de operação do dispositivo pelo mesmo período, e em alguns casos devem ser usado relés de proteção adicional ao circuito.
  *  O equipamento foi projetado para instalação dentro de caixas 4x4 no forro ou laje coberta e somente poderá trabalhar com conectores compatíveis com os procedimentos de segurança.
  *  Não conecte o equipamento a cargas maiores que os valores recomendados.
  *  Conecte o equipamento de acordo com os diagramas apresentados no manual.
  *  Conexões erradas ou inapropriadas podem ser perigosas.

##1. Informações Gerais Sobre o Sistema @HOME
**@home** é um sistema sem fios, com base na tecnologia de nRFWTI. **@home** oferece muitas vantagens quando comparado com sistemas similares. Em geral, os sistemas de rádio criam uma conexão direta entre o receptor e transmissor. Entretanto, o sinal de rádio é enfraquecida por uma variedade de obstáculos localizados no seu caminho (paredes do apartamento, mobiliário, etc.) e em casos extremos, incapaz de transferir dados necessários. A vantagem do sistema **@home** é que os seus dispositivos além de ser transmissores e receptores de sinais, também são “repetidores” de sinal. Quando um caminho de ligação direta entre o transmissor e o receptor pode não ser estabelecido, a ligação pode ser estabelecida através de outros dispositivos intermediários.

**@home** é um sistema bidirecional. Isso significa que o sinal não apenas é transmitido para os receptores, mas também os receptores enviam a confirmação da sua recepção. Esta operação confirma seu status de modo a verificar se eles estão ativos.
**@home** opera na faixa de frequência de 2.4Ghz para transmissão de dados. Cada rede **@home** tem o seu próprio número de identificação exclusivo (NET ID), além de um canal específico dentro da faixa definida, razão pela qual é possível cooperar dois ou mais sistemas independentes em um único edifício, sem qualquer interferência.

O sistema **@home** gera uma estrutura de rede dinâmica. Logo após que o sistema **@home** é ligado, a localização de cada um dos componentes é automaticamente atualizada em tempo real, através de confirmação do estado dos sinais recebidos a partir de dispositivos que operam em rede _**"mesh"**_.

O módulo de atuadores **@home** foi projetado para ligar e/ou desligar dispositivos conectados aos seus terminais usando ondas de rádio, ou pulsadores e interruptores diretamente conectados ao equipamento.

##2. Instalando o Módulo

<img src="/imagens/perigo.de.choque.png" height="40" witdh="40"> Perigo de choque elétrico !
------------ 
  * Antes de ligar o  equipamento na rede elétrica, certifique-se de que a voltagem é compatível com a indicada no produto (110V ou 220V). Caso a voltagem não seja compatível, poderá provocar danos ao produto e prejudicar a sua segurança pessoal.
  * Para evitar sobrecarga elétrica, não ligue o equipamento utilizando benjamins ou extensões, evitando, assim, danificar os componentes do produto e provocar sérios acidentes.
  * Instale o módulo de atuadores no local determinado.
  * Conecte o módulo B3R3PRF conforme o diagrama a seguir.


Notas | Diagrama
------------ | -------------
**N** | Terminal do Neutro  
**F** | Terminal do Fase  
**C** | Comum  
**R1**| Terminal de saída para a carga 1 
**R2**| Terminal de saída para a carga 2  
**R3**|Terminal de saída para a carga 3
**P1**| Chave de contato 1 
**P2**| Chave de contato 2  
**P3**| Chave de contato 3
**GND**|Comum para as chaves de contato


**Módulo de 3 cargas ligadas em VAC e três pulsadores**

<img src="/imagens/B3R3PRF1.png" height="400" witdh="40">

**Opção com fonte alternativa para as  cargas**

<img src="/imagens/B3R3PRF2.png" height="400" witdh="40">

<img src="/imagens/i.png" height="40" witdh="40">  Dicas para ajuste da antena
------------
  * A antena é localizada na parte interna do equipamento e é sinalizada na etiqueta de identificação do produto. Desta forma, deve-se sempre instalar o equipamento com a etiqueta de identificação voltada para o ambiente a ser controlado.
  * Superfícies de metal próximas à antena, podem impactar na recepção do sinal.
  * Reatores ou motores próximos à antena, podem impactar na recepção do sinal.
  * Lajes de concreto podem impactar na recepção do sinal.

##3. Operação Básica

O módulo B3R3PRF é formado por 3 relés de acionamento de cargas e 3 chaves de contato que podem enviar comandos para estes relés ou para qualquer outro equipamento na rede **@home**.

Cada uma das 3 chaves de contato **P1**, **P2** ou **P3** podem operar no modo pulsador ou no modo interruptor. O modo de fábrica é o modo pulsador que consiste em acionar a chave de contato por um tempo mínimo pré-determinado, para que o cenário correspondente possa ser executado. Neste modo, cada pulsador possui um cenário associado a função _**“short press”**_, um cenário associado a função _**“long press”**_ e um cenário especial chamado _**“panic”**_:

* Acionamento _**“short press”**_ - Quando o pulsador é acionado por um tempo menor que 500ms.
* Acionamento _**“long press”**_ - Quando o pulsador é acionado por um tempo maior que 500ms e menor que 4seg.
* Botão de _**“panic”**_ - Quando o pulsador é acionado por um tempo maior que 4seg.

As chaves de contato já vem configurado de fábrica da seguinte forma:

_**“short press”**_ no pulsador **P1** – Inverte a carga **R1** (Cenário **A1**)  
_**“short press”**_ no pulsador **P2** – Inverte a carga **R2** (Cenário **A2**)  
_**“short press”**_ no pulsador **P3** – Inverte a carta **R3** (Cenário **A3**)  
_**“long press”**_ no pulsador **P1** – Liga as 3 cargas  (Cenário **B1**)  
_**“long press”**_ no pulsador **P2** – Desliga as 3 cargas (Cenário **B2**)  
_**“long press”**_ no pulsador **P3** – Desliga as 3 cargas (Cenário **B3**)  
_**“panic”**_ em qualquer pulsador – Envia comando especial à central Net Center caso a mesma esteja presente na rede.

O modo interruptor consiste em executar o cenário de _**“short press”**_ quando a chave de contato é acionada e o cenário de _**“long press”**_ quando a chave de contato é liberada, semelhante ao botão liga e desliga.

<img src="/imagens/i.png" height="40" witdh="40">  Informações!
------------
  * É possível alterar a configuração de fábrica através do computador utilizando o adaptador para porta USB que é vendido separadamente ou através de outro equipamento ligado na mesma (NET ID).
  * Para utilizar a comunicação com o computador é necessário além do adaptador para porta USB, a instalação do programa de comunicação com portas Seriais. A configuração da porta serial deve ser: **57600, N, 8, 1**.

##4. Comunicando o Equipamento com Outros Módulos

É possível associar vários equipamentos do sistema **@home** permitindo criar uma rede de equipamentos, cujo principal objetivo é criar cenários complexos e ampliar o alcance da rede. Esta associação pode ser feita mesmo sem a necessidade da central Net Center:

1. Configure cada um dos equipamentos com um endereço diferente mas na mesma (**NET ID**) para que seja possível que os equipamentos interajam entre si.

2. Posicione os equipamentos de tal forma que nenhum equipamento fique fora do alcance de pelo menos um dos equipamentos que se deseja interligar.

3. Altere os cenários pré-determinados para realizar as cenas desejadas.

<img src="/imagens/i.png" height="40" witdh="40">  Informações
------------
  * É possível alterar a maioria das funções de controle e comando dos equipamentos **@home** sem a necessidade da central Net Center.
  * É possível configurar todas as funções dos equipamentos através do computador e do adaptador USB.
  * A central Net Center é necessária quando se deseja controlar os equipamentos através de smartphones ou tablets ou executar cenas em horários pré-determinados.

##5. Cénarios

O módulo **B3R3PRF** pode armazenar até 16 cenários diferentes divididos em 3 bancos chamados: Banco **A**,  Banco **B** e Banco **S**. Os cenários podem ser executados através das chaves de contato como também por outros equipamentos ligados na rede **@home**.

O banco **A**, possui 3 posições para cenários chamados **A1**, **A2** e **A3**. Estes cenários estão diretamente relacionamento com as chaves de contato **P1**, **P2** e **P3** respectivamente. Quando o equipamento está no modo “pulsador” estes cenários são executados quando é acionado o “short press” na respectiva chave de contato. No modo interruptor este cenário é executado quando a chave de contato respectiva é acionada.

O banco **B**,  possui 3 posições para cenários chamados **B1**, **B2** e **B3**. Estes cenários estão diretamente relacionados com as chaves de contato **P1**, **P2** e **P3** respectivamente. Quando o equipamento está no modo “pulsador” estes cenários são executados quando é acionado o “long press” na respectiva chave de contato. No modo interruptor este cenário é executado quando a chave de contato respectiva é liberada.

O banco **S**, possui 10 posições para cenários chamados **S0** a **S9**. Estes cenários não estão associados diretamente as chaves de contato e podem ser executados através do computador, por outros cenários, como também por outros equipamentos na rede **@home**.

<img src="/imagens/i.png" height="40" witdh="40">  Informações
------------
  * Cada cenário pode armazenar um máximo de 23 caracteres. Como um comando básico possui de 3 a 5 caracteres, cada cenário pode armazenar de 5 a 8 comandos. Cada comando deve ser separado pelo caractere “;”. 
  * É possível encadear cenários, aumentando consideravelmente a quantidade de comandos executados por vez.

  * Exemplo de cenários:

    * **“I1”** - Inverte a carga R1  
    * **“DT”** - Desliga as cargas R1, R2 e R3  
    * **“I1;L2”** - Inverte a carga R1 e liga a carga R2  
    * **“S0”** - Executa o cenário S0  
    * **“30:L1”** - Envia para o equipamento cujo endereço é 30, o comando “L1”  

##6. Comandos 

Os seguintes comandos estão disponíveis no módulo B3R3PRF podendo ser enviados através das chaves de contato, do conector de programação ou de outros equipamentos, como também da central Net Center.

Se os comandos forem enviados através do conector de programação, ao final de cada grupo de comandos deve ser enviado o caractere **LF** (Line Feed ou Chr(10))

#####Os comandos seguem o formato:

  _**comando parametro1 parametro2 parametro3 parametro4**_ onde os parâmetros podem ser opcionais dependendo do tipo de comando.

Para enviar comandos para outros equipamentos, deve-se informar o endereço do equipamento destino, sempre com 2 caracteres, seguido do caractere “**:**” antes do comando a ser enviado:

#####Exemplo:
**30:L1** - Envia para o equipamento cujo endereço é 30, o comando “L1”  

Para enviar multiplos comandos para outros equipamentos de uma única vez, deve-se colocar os comandos entre aspas e separá-los pelo caractere "**;**"

#####Exemplo:
**30:"L1;L2"** - Envia para o equipamento cujo endereço é 30, o comando "L1;L2"

###Grupo 1 – Comandos de operação das cargas**

#### **L1**, **L2** , **L3**, **LT**, **D1**, **D2**, **D3**, **DT**, **I1**, **I2**, **I3**, **IT**, **P1**, **P2**, **P3**

Comandos para liga, desliga, inversão e pulso de cargas nos relés:

* **L1**, **L2**, **L3** ou **LT** -  Liga as cargas R1, R2, R3 ou todas respectivamente.  
* **D1**, **D2**, **D3** ou **DT** - Desliga as cargas R1, R2, R3 ou todas respectivamente.  
* **I1**, **I2**, **I3** ou **IT** - Inverte as cargas R1, R2, R3 ou todas respectivamente.  
* **P1**, **P2** ou **P3** - Pulsa as cargas R1, R2 ou R3 respectivamente. _**(*)**_  

**Parâmetros disponíveis** (exceto para os comandos P1, P2 ou P3)  

* _**tempo**_  - Tempo em segundos que esta carga ficará no estado selecionado. (valores entre 0 e 65534 seg)
* _**retornarPara**_ - Situação para a qual o relé irá retornar após o tempo pré-determinado:  
  * _**0**_  Retornar para desligado  
  * _**1**_  Retornar para ligado  
  * _**2**_  Inverter o estado da carga  
  * _**3**_  Retornar para o estado anterior ao comando  
  
_**(*)**_ _Pulsar significa ligar e desligar as cargas rapidamente 10 vezes tendo seu estado final como desligado._

###Grupo 2 – Comandos gerais de configuração do rádio e da rede

####$RAD

Endereço e outros parâmetros do rádio nRFWTI.

**Parâmetros disponíveis** 

* _**endereço**_ - Endereço único na rede, no formato hexadecimal (**Default**: 88 – valores entre 00 e FE).   
* _**frequênciaRF**_ - Variação em 1Mhz da frequência de operação do rádio no intervalo de 2400Mhz a 2525Mhz, seguindo a fórmula: 2400 + _**frequênciaRF**_ (**Default**: 76 – valores entre 0 e 125).  
* _**roteador**_ - Ativa ou desativa a função de roteador, que faz com que o rádio retransmita pacotes dentro da rede: (**Default**: 0).  
  * _**0**_  - Não funciona como roteador  
  * _**1**_  - Funciona como roteador  
* _**somenteTransmite**_ - Muda o modo de transmissão para transmisão ou transmissão/recepção (**Default**: 0)  
  * _**0**_  - Transmite e recebe
  * _**1**_  - Somente Transmite 

####$NET

NET ID e endereço da Central Net Center. _**(*)**_

**Parâmetros disponíveis**
* _**central**_ - Endereço único da central Net Center, no formato hexadecimal.(**Default**: FF – valores entre 00 e FF). _**(\*\*)**_ 
* _**offset1**_  - Primeiro byte do NET ID, no formato hexadecimal (**Default**: 69 – valores entre 00 e FF).  
* _**offset2**_  - Segundo byte do NET ID, no formato hexadecimal (**Default**: 5A – valores entre 00 e FF).  
* _**offset3**_  - Terceiro byte do NET ID, no formato hexadecimal (**Default**: 3C – valores entre 00 e FF).

_**(*)**_ _O endereço NET ID é formado por 3 bytes e deve ser igual para todos os equipamentos de uma mesma rede. Mesmo que outra rede esteja na mesma frequência de rádio, o NET ID vai garantir que haja uma independência entre elas. **NUNCA DEIXE SEU NET ID COM OS PADRÕES DE FÁBRICA.**_  
_**(\*\*)**_ _O endereço **FF** significa que não existe uma central Net Center na rede._  

####$PAR

Parâmetros de transmissão do rádio.

**Parâmetros disponíveis**|
* _**potência**_  - Potência de transmissão (**Default**: 3)
  * _**0**_ - Mínima
  * _**1**_ - Média
  * _**2**_ - Alta
  * _**3**_ - Máxima
  
* _**velocidade**_ - Velocidade de transmissão  (**Default**: 2)
  * _**0**_ - 1 Mbps
  * _**1**_ - 2 Mbps
  * _**2**_ - 250 Kbps
  * 
* _**tamanhoCRC**_ - Quantos bytes ocupa o CRC “Controle de Checagem de Erro” em cada pacote transmitido (**Default**: 2)
  * _**0**_ - Desabilitado  
  * _**1**_ - 8 bits  
  * _**2**_ - 16 bits  

####$RET

Parâmetros de retransmissão do rádio. _**(*)**_

**Parâmetros disponíveis**|

* _**atraso**_ - Atraso entre as retransmissões, em múltiplos de 4ms, no caso de falha (**Default**: 4, valores entre 0 e 15)
* _**quantidade**_ – Quantidade de retransmissões (**Default**: 4, - valores entre 0 e 15).

_**(*)**_ _A partir do firmware **2.7** este comando não possui mais utilidade, estando ainda listado por questão de compatibilidade_

####$NEA

Os dispostivos da rede **@home**, possuem a capacidade de encontrar outros dispositivos próximos, permitindo assim que a rede _**"mesh"**_ funcione corretamente. Em algumas ocasiões especiais é necessário informar o endereço dos equipamentos próximos desabilitando-se assim a função _auto-discover_.

**Parâmetros disponíveis**
* _**endereço1 a 4**_ - Endereço de um equipamento próximo , no formato hexadecimal (**Default**: FF – valores entre 00 e FF) _**(*)**_ .

_**(*)**_ _O endereço **FF** não é associado a nenhum equipamento e deve ser utilizado quando se deseja retornar ao modo auto-discover: **$NEA FF FF FF FF**_

<img src="/imagens/i.png" height="40" witdh="40">  Dicas para Configuração !
-----------------
  * A maioria dos comandos de configuração do rádio e da rede já vem pré-definidos de fábrica para seu melhor desempenho. **Não é necessário nenhum ajuste adicional.**
  * O endereço do rádio, o NET ID e o canal do rádio por estarem com seus parâmetros default, devem ser alterados para evitar interferência com outros equipamentos ou outras redes. Comandos **$RAD** e **$NET**.
  * Pode-se usar o caractere “?” quando não se deseja alterar o valor de um determinado parâmetro: 
    * Ex: **$RAD ? 77** – O endereço do rádio permanece inalterado, e a frequência do rádio foi alterado para o canal 77.
  * Após qualquer alterações nas configurações é necessário salvá-las e reinicializar o equipamento para que as mesmas surtam efeito. Utilize **$SAV** e **$RST** respectivamente.

**Grupo 3 – Outros comandos gerais**

####$SAV
  Salva os parâmetros configurados na memória não volátil (EEPROM)

####$STA
  Envia os parâmetros configurados para a porta de configuração caso o comando tenha sido recebido por ela, ou para o equipamento requisitante.
  
####$SCE
Envia os cenários cadastrados para a porta de configuração caso o comando tenha sido recebido por ela, ou para o equipamento requisitante caso tenha havido a solicitação de um cenário específico.

**Parâmetros disponíveis**
* _**banco**_ - Número do banco que se deseja mostrar. (*Default*: todos – valores 1, 2 ou 3 para os bancos A, B e S respectivamente).  
* _**cenario**_ - Número do cenário que se deseja mostrar dentro do banco especificado. (Default: 0 – valores 0 até o total de cenários do banco) _**(*)**_. 
  
_**(*)**_ _Os bancos **A** e **B** têm início a partir do cenário 1 e o banco **S** inicia-se a partir do cenário 0 (zero)._

####$FDF

Retorna todos os parâmetros do equipamento para os ajustes de fábrica e executa um reset geral. 

####$RST

Reinicia o equipamento.

###Grupo 4 – Comandos específicos para o módulo B3R3PRF

####$DEL

Tempos de configuração do _**“short press”**_ e do _**“long press”**_.

**Parâmetros disponíveis**|
* _**maximoShortPress**_ - Tempo máximo em ms que uma chave de contato deve ser ativada para que seja considerado como _**“short press”**_. (**Default**: 400ms – Valores entre 1 e 65535 ms).
* _**minimo Panic**_ - Tempo mínimo em ms que uma chave de contato deve ser ativada para que seja considerado como um _**“panicPress”**_. (**Default**: 4000ms – Valores entre _**“maximoShortPress”**_ e 65535 ms) _**(*)**_.
* _**minimoValido**_ - Tempo mínimo em ms que uma chave de contato deva ser ativada para que qualquer tipo de acionamento deva ser considerado. (**Default**: 25ms – Valores entre 0 e _**maximoShortPress**_ ms).

_**(*)**_ _No modo pulsador, o cenário é executado somente após a chave de contato ter sido liberada_  
_**(*)**_ _O **“long press”** é considerado, quando o tempo de acionamento é maior que o **maximoShortPress** e menor que **minimoPanic**._

####$REL

Configura o modo com que a carga de cada relé irá retornar após uma queda de energia

**Parâmetros disponíveis**

* _**retornoCarga1 a 3**_ - Situação de retorno de cada carga: (Default: 400ms – Valores entre 1 e 65535 ms).
  * _**0**_ - Carga desligada
  * _**1**_ - Carga ligada
  * _**2**_ - Situação antes da queda de energia. Ex: **$REL 0 1 2**.

####$BUT

Configura o modo como as chaves de contato devem funcionar.

**Parâmetros disponíveis**|
* _**tipoChave1 a 3**_  - Modo de cada chave de contato
  * _**0**_ - Modo interruptor
  * _**1**_ -  Modo pulsador

##Grupo 5 – Comandos para cenários

####A1, A2, A3, B1, B2, B3, S0, S1, S2, S3, S4, S5, S6, S7, S8 e S9

Executa um cenário. Os cenários **A** e **B** também estão associados às chaves de  contato mas funcionam como qualquer outro cenário e podem ser chamados através de outros cenários ou remotamente por outros equipamentos. 

####WA1, WA2, WA3 ,WB1 ,WB2 ,WB3 ,WS0 ,WS1 ,WS2 ,WS3 ,WS4 ,WS5 ,WS6 ,WS7 ,WS8 ,WS9

Grava um cenário na memória não volátil (EEPROM)

**Parâmetros disponíveis**|

* _**comandos**_ - Comandos que serão executados pelo cenário específico. Caso seja necessário a execução de mais de um comando, é necessário separar cada comando pelo caractere “;” e o colocar o conjunto inteiro entre aspas duplas. Caso esteja gravando um cenário em um equipamento remoto e este cenário possua mais de um comando é preciso envolver estes comandos entre aspas simples e o comando completo após o endereço entre aspas duplas: 
  * Ex: _**WA1 L1**_ ou _**WA2 “L1;L2”**_ ou _**WS0 “I3;A1”**_.
  * Ex: _**30:WA1 B1**_ ou _**30:"WA1 'L1;L2'"**_

##7. Procedimentos para Mau Funcionamento

O equipamento não responde a uma transmissão remota:

* Verifique se o alcance máximo não foi excedido e que o sinal não está obstruído por superfícies ou caixas de metal. O led ACT pisca em intervalos constantes, mas quando um comando válido é recebido a frequência da piscada muda por alguns segundos. Verifique se o módulo está recebendo comandos corretamente através da visualização do led ACT.

* Caso o equipamento tenha sido reiniciado recentemente, envie alguns comando adicionais para que a memória dos equipamentos remotos limpe qualquer referência de informação deste equipamento. 

##8. Ajustes de Fábrica
Caso necessário, é possível ajustar o equipamento para os padrões de fábrica. Insira um objeto pontiagudo no orifício situado ao lado do conector de programação, exercendo uma leve pressão. Aguarde 5 segundos com o objeto inserido e verifique se o led ACT ficou aceso por 2 segundos. O equipamento ira resetar com os parâmetros de fábrica configurados. 

##9. Garantia

##### I - Prazo e Comprovação da Garantia

  * O produto abaixo identificado, devidamente lacrado, é garantido pelo seu fabricante e/ou importador (XSOLUTIONS S.A.), pelo prazo de um ano, contado a partir da data de sua aquisição pelo primeiro consumidor e obedecidas as condições e as recomendações especiais aqui discriminadas.

  * Esta garantia contratual é dada ao produto abaixo identificado, exclusivamente contra eventuais defeitos decorrentes de projeto, fabricação, montagem, ou quaisquer outros vícios de qualidade que o tornem impróprio ou inadequado ao uso regular.

  *  Para a comprovação desse prazo, o consumidor deverá apresentar este Termo de Garantia, devidamente preenchido, e/ou a 1ª via da nota fiscal de compra, ou outro documento fiscal equivalente, desde que identifique o produto.
Exija do estabelecimento comercial revendedor, o preenchimento correto deste Termo de Garantia.

##### II - Exclusão da Garantia

A garantia não abrangerá, sendo, pois, ônus do consumidor:

* Os danos sofridos pelo produto, ou seus acessórios, em consequência de acidente, maus tratos, manuseio ou uso incorreto e inadequado;

* Os danos sofridos pelo produto, em consequência de sua utilização para finalidades diversas das especificadas pelo fabricante e/ou importador (XSOLUTIONS S.A.), ou incompatíveis com a destinação do mesmo.

##### III - Local Onde a Garantia Deverá ser Exercitada

  * Os consertos em garantia somente deverão ser efetuados por uma Assistência Autorizada, devidamente nomeada pelo fabricante e/ou importador (XSOLUTIONS S.A.), que, para tanto, se utilizará de técnicos especializados e de peças originais, relacrando o seu aparelho e garantindo o serviço executado.

##### IV - Cessação da Garantia

  *  Não confie o conserto do produto abaixo identificado a curiosos, pessoas ou oficinas não autorizadas e não credenciadas pelo seu fabricante e/ou importador (XSOLUTIONS S.A.).

  *  Se isto vier a ocorrer, com a consequente violação do lacre do produto, a garantia cessará, de imediato.

  * O produto abaixo identificado foi projetado para funcionamento em uso doméstico, única e exclusivamente. A sua utilização, para uso não doméstico, industrial ou comercial, acarretará a cessação imediata da garantia.


##### V - Recomendações Especiais

  * Antes de colocar o produto em funcionamento, leia atentamente as instruções de uso e/ou instalação contidas no próprio aparelho, na embalagem, ou no manual respectivo. Siga-as rigorosamente. Elas são a sua segurança.

  * Certifique-se de que a voltagem a ser utilizada é a mesma indicada no aparelho (110V a 220V). Verifique se a instalação elétrica do local está correta e adquada.

  * Para evitar danos, mantenha o produto bem armazenado e limpo, em ambiente protegido das intempéries (chuva, vento, umidade, raios solares, etc.).

  * Não introduza quaisquer objetos estranhos à função própria do produto, principalmente quando este estiver em funcionamento, evitando acidentes.

#####VI - Fabricante e/ou Importador

_**XSOLUTIONS S.A.  
CNPJ/M.F. Nº 61.064.978/0001-01  
Av. Carlos Vasconcelos, 1702 – Aldeota – Fortaleza/CE**_

Qualquer reclamação, comentário ou sugestão sobre o atendimento e os reparos prestados pelas Assistências Autorizadas, ligue ao nosso Serviço de Atendimento ao Consumidor.

Departamento de Assistência Técnica:(85) 3311.6464.
