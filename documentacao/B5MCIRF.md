# B5MCIRF
#### Módulo de 4 medidores de corrente em série até 30A

## Manual de operação  
O módulo de medidores é projetado para operar em locais onde a medição de corrente elétrica AC em circuitos até 30A 
é necessária. Este módulo **SEMPRE** envia as suas informações para a central NetCenter, desta forma é imprescindível a
existência da referida central na mesma rede na qual o equipamento foi configurado para que as informações possam ser
visualizadas.

Leia atentamente as recomendações e instruções de uso.

##Especificações
Item | Descrição 
------------ | -------------
**Alimentação** | 110/220v
**Consumo nominal** | 4ma
**Comunicação** | Rádio frequência 2.4Ghz, 127 canais adicionais, endereçamento de 24bits
**Protocolo** | @home
**Sensores** | 4 medidores de corrente ACS712 de 30A
**Cenas** | 10 cenas 
**Umidade** | +5% a 95% não condensado
**Temperatura de operação** |-10°C a +70°C

##Informações Técnicas 

 * Controlado pelos sistemas *@home*  
 * Microcontrolado  
 * Tipo de medição: watts  
 * O dispositivo pode ser operado remotamente  

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
  * Conecte o módulo B4MCS3RF conforme o diagrama a seguir
  * Cada um dos 4 circuitos a serem medidos precisa ser conectado duas vezes ao módulo B4MCS3RF. A primeira conexão é o fio que
  vem do quadro de alimentação que deve ser conectada à uma das 4 entradas do medidor. A segunda conexão é a que sai do medidor em 
  direção aos equipamentos, fazendo-se assim que o equipamento fique ligado em série com este circuito.


Notas | Diagrama
------------ | -------------
**N** | Terminal do Neutro  
**F** | Terminal do Fase  
**e1** | Entrada da medição do circuito 1  
**e1** | Saída da medição do circuito 1  
**e2** | Entrada da medição do circuito 2 
**e2** | Saída da medição do circuito 2
**e3** | Entrada da medição do circuito 3  
**e3** | Saída da medição do circuito 3
**e4** | Entrada da medição do circuito 4  
**e4** | Saída da medição do circuito 4

**Ligação padrão para medição de 4 circuitos**

<img src="/imagens/B4MCS3RF1.png" height="400" witdh="40">

<img src="/imagens/i.png" height="40" witdh="40">  Dicas para ajuste da antena
------------
  * A antena é localizada na parte interna do equipamento e é sinalizada na etiqueta de identificação do produto. Desta forma, deve-se sempre instalar o equipamento com a etiqueta de identificação voltada para o ambiente a ser controlado.
  * Superfícies de metal próximas à antena, podem impactar na recepção do sinal.
  * Reatores ou motores próximos à antena, podem impactar na recepção do sinal.
  * Lajes de concreto podem impactar na recepção do sinal.

##3. Operação Básica

O módulo B4MCS3RF é formado por 4 medidores de corrente em série, cujo objetivo é medir a corrente em Ampéres que passa por
cada um destes medidores, calcular a potência em Watts referente a cada circuito e enviá-la para a central NetCenter para 
armazenagem.

A medição em série significa que cada circuito deve entrar e sair do módulo pelas suas respectivas portas e[1,2,3,4] para que
a medição seja feita correntamente.

Cada circuito não pode ultrapassar a carga limite da porta que é de 30A, caso contrário danos podem ser causados ao equipamento.

É possível em teoria medir cargas maiores de 30A, utilizando-se do recurso de agrupamento de portas. Ver comando **$GRP**. Neste caso o mesmo circuito deve entrar e sair em mais de uma porta, de forma paralela, dividindo-se assim a corrente resultante entre as várias portas.

<img src="/imagens/perigo.de.choque.png" height="40" witdh="40"> Perigo de curto-circuito !
------------
 * Nunca misture os fios de circuitos diferentes nas respectivas entradas e saídas e1, e2, e3 e e4, pois isso provavelmente 
 causará danos irreparáveis ao equipamento, podendo também dependendo do tipo de equipamento ligados nestes circuitos, 
 provocar curto-circuitos e danos nestes.
 
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

O módulo **B4MCS3RF** pode armazenar até 10 cenários diferentes armazenados em um banco chamado: Banco **S**. 
Os cenários podem ser executados por outros equipamentos ligados na rede **@home**.

O banco **S**, possui 10 posições para cenários chamados **S0** a **S9**. 

<img src="/imagens/i.png" height="40" witdh="40">  Informações
------------
  * Cada cenário pode armazenar um máximo de 23 caracteres. Como um comando básico possui de 3 a 5 caracteres, cada cenário pode armazenar de 5 a 8 comandos. Cada comando deve ser separado pelo caractere “;”. 
  * É possível encadear cenários, aumentando consideravelmente a quantidade de comandos executados por vez.

  * Exemplo de cenários:

    * **“S1”** - Executa o cenário S1 
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

###Grupo 1 – Comandos de operação

**Este módulo não possui comandos no Grupo 1, haja visto que o mesmo não possui atuadores**

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

####$ENA

Habilita o monitoramento em cada uma das 4 portas do módulo.

**Parâmetros disponíveis**

* _**portaHabilitada1 a 4**_ - Habilita ou desabilita o monitoramento da cada porta (**Default**: 1 – Valor entre 0 e 1).
  * _**0**_ - Porta desabilitada
  * _**1**_ - Porta habilitada


####$VCA

Configura um valor fixo de voltagem em corrente alternada para cada porta, que será multiplicado com o valor da corrente medido para obtenção do cálculo da potência em watts.

**Parâmetros disponíveis**

* _**valorVCA1 a 4**_ - Valor da voltagem considerada para cálculo da potência em cada porta: (**Default**: 220V – Valores entre 0 e 65535V).

####$MCU

Configura o menor de valor de corrente medido a ser considerado válido. Qualquer valor medido abaixo desse valor será desconsiderado. Este valor é medido em milliamperes.

**Parâmetros disponíveis**
* _**valorMinimo1 a 4**_  - Valor minimo de corrente que é considerado válido por porta: (**Default**: 160 – Valores entre 0 e 65535ma).

####$SEC

Configura o tempo de envio para a central NetCenter do valor médio da corrente medida por porta.

**Parâmetros disponíveis**
* _**tempoEnvio1 a 4**_  - Tempo em segundos para envio dos dados de leitura para a central NetCenter: (**Default**: 120 – Valores entre 0 e 65535 segundos).

####$CUR

Envia o valor da corrente medida média e atual para o solicitante. Caso este comando tenha sido digitado via interface serial
o valor é enviado para a interface serial. Caso senha sido solicitado pela rede, o mesmo é retornado para o endereço 
solicitante

**Parâmetros disponíveis**

* _**porta**_  - Porta da qual se deseja obter a leitura (Valores entre 0 e 3, respectivamente para as portas 1 a 4). 

#####Exemplo: 
**30:$CUR 0** - Solicitado equipamento cujo endereço é 30 o valor da corrente média e atual da porta  1  

####$GRP

Habilita o agrupamento de portas na qual várias portas terão as suas medição somadas e transmitidas como se fossem uma única porta.

**Parâmetros disponíveis**|
* _**tipoAgrupamento**_  - Tipo de Agrupamento (**Default**: 1)
  * _**1**_ - 4 portas independentes (1 2 3 4)
  * _**2**_ - Portas  1 e 2 agrupadas, portas 3 e 4 independentes (1+2 3 4)
  * _**3**_ - Portas 1, 2 e 3 agrupadas, porta 4 independente (1+2+3 4)
  * _**4**_ - Portas 1,2,3 e 4 agrupadas (1+2+3+4)
  * _**5**_ - Portas 1 e 2 agrupadas no grupo1, portas 3 e 4 agrupadas no grupo 2 (1+2 3+4)

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
