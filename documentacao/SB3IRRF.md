#SB3IRRF
####Módulo de 3 infravermelhos para multimídia

##Manual de operação
O módulo de emissão de IR foi projetado para controlar equipamentos que utilizem a tecnologia de infravermelho para sua operação, tais como TV, ar-condiconados, receivers, etc. É igualmente possível enviar um sinal para qualquer módulo que possa ser integrado com o Sistema wti@home. Leia atentamente as recomendações e instruções de uso. 

##Especificações
Especificações | Técnicas 
------------ | -------------
**Alimentação** | 110/220v
**Consumo nominal** | 4ma
**Comunicação** | Rádio frequência 2.4Ghz, 127 canais adicionais, endereçamento de 24bits
**Protocolo** | @home
**Portas disponíveis** | 3  (1 fixa e 2 através de cabos extensores)
**Frequência de IR** | 35Khz a 45Khz
**Cenas** | 20
**Umidade** | +5% a 95% não condensado
**Temperatura de operação** |-10°C a +70°C
**Função pânico** | NÃO

##Informações Técnicas 

 * Controlado pelo sistema wti@home;  
 * Microcontrolado;  
 * Tipo de acionamento: emissor de IR;
 * O dispositivo pode ser operado remotamente ou por pulsadores e interruptores convencionais.

<img src="/imagens/perigo.de.choque.png" height="40" witdh="40"> Perigo|Choque elétrico !
------------ | -------------
  * | Todos os trabalhos no dispositivo só podem ser executados por um eletricista ou pessoa qualificada. Observe os regulamentos nacionais.
  * | Mesmo quando o dispositivo está desligado, a tensão pode estar presente nos seus terminais. Qualquer obra que introduza alterações nas configurações de conexões ou à carga, deve ser sempre realizada com a rede elétrica desligada.

<img src="/imagens/i.png" height="40" witdh="40">  Informações| Informações!
------------ | -------------
  * |O equipamento foi projetado para instalação em ambientes protegidos, dentro de caixas 4x4 no forro ou laje coberta e somente poderá trabalhar com conectores compatíveis com os procedimentos de segurança.
  * | Conecte o equipamento de acordo com os diagramas apresentados no manual..
  * | Conexões erradas ou inapropriadas podem ser perigosas.

##1. Informações Gerais Sobre o Sistema @HOME
@home é um sistema sem fios, com base na tecnologia de nRFWTI. @home oferece muitas vantagens quando comparado com sistemas similares. Em geral, os sistemas de rádio criam uma conexão direta entre o receptor e transmissor. Entretanto, o sinal de rádio é enfraquecida por uma variedade de obstáculos localizados no seu caminho (paredes do apartamento, mobiliário, etc.) e em casos extremos, incapaz de transferir dados necessários. A vantagem do sistema @home é que os seus dispositivos além de ser transmissores e receptores de sinais, também são “repetidores” de sinal. Quando um caminho de ligação direta entre o transmissor e o receptor pode não ser estabelecido, a ligação pode ser estabelecida através de outros dispositivos intermediários.

@home é um sistema sem fio, ou seja, bidirecional. Isso significa que o sinal não apenas é transmitido para os receptores, mas também os receptores enviam a confirmação da sua recepção. Esta operação confirma seu status de modo a verificar se eles estão ativos.
@home opera na faixa de frequência de 2.4Ghz para transmissão de dados. Cada rede @home tem o seu próprio número de identificação exclusivo (NET ID), além de um canal específico dentro da faixa definida, razão pela qual é possível cooperar dois ou mais sistemas independentes em um único edifício, sem qualquer interferência.

O sistema @home gera uma estrutura de rede dinâmica. Logo após que o sistema @home é ligado, a localização de cada um dos componentes é automaticamente atualizada em tempo real, através de confirmação do estado dos sinais recebidos a partir de dispositivos que operam em rede "mesh".

O módulo de emissão de IR @home foi projetado para controlar equipamentos via Infravermelho que estejam em seu campo de atuação, usando ondas de rádio.

##2. Instalando o Módulo

<img src="/imagens/perigo.de.choque.png" height="40" witdh="40"> Perigo|Choque elétrico !
------------ | -------------
  * | Antes de ligar o  equipamento na rede elétrica, certifique-se de que a voltagem é compatível com a indicada no produto (110V ou 220V). Caso a voltagem não seja compatível, poderá provocar danos ao produto e prejudicar a sua segurança pessoal.
  * | Para evitar sobrecarga elétrica, não ligue o equipamento utilizando benjamins ou extensões, evitando, assim, danificar os componentes do produto e provocar sérios acidentes.
  * |Conecte o módulo à fonte de alimentação 12V enviada em conjunto.
  * |Instale o módulo de emissão de IR no local determinado a fim de que o seu emissor principal ou os seus emissores secundários através do cabo de extensão tenham visa direta ao módulo receptor do equipamento que se deseja controlar.

<img src="/imagens/1SB3IRRF.png" height="400" witdh="40">

**Dicas para Ajustes da Antena**

<img src="/imagens/i.png" height="40" witdh="40">  Antena| Antena!
------------ | -------------
  * |A antena é localizada na parte interna do equipamento e é sinalizada na etiqueta de identificação do produto. Desta forma, deve-se sempre instalar o equipamento com a etiqueta de identificação voltada para o ambiente a ser controlado.
  * | Superfícies de metal próximas à antena, podem impactar na recepção do sinal.
  * | Reatores ou motores próximos à antena, podem impactar na recepção do sinal.
  * | Lajes de concreto podem impactar na recepção do sinal.

##3. Operação Básica

O módulo SB3IRRF é formado por 3 emissores de sinais Infravermelhos para controle de equipamentos que utilizem esta tecnologia, que podem ser acionados através de pulsadores remotos ou  qualquer outro equipamento na rede @home.

Emissores de infravermelho são leds normais com uma cor particular. Nós humanos não podemos ver sua cor porque seu tamanho de onda está na faixa dos 950 nm que é abaixo do espectro visível. 

Uma transmissão em infravermelho usa o conceito de “marcas” e “espaços”. Nenhuma luz é emitida durante um “espaço”. Durante uma “marca”, o emissor de IR pulsa em uma determinada frequência. Frequências de 30kHz a 60kHz são usadas em equipamentos eletrônicos. A mais comum é 38kHz.

Cada conjunto de “marca” e “espaço” pode representar geralmente: o início da transmissão, um “1”, um “0” ou o final da transmissão. Cada fabricante utiliza um padrão de mercado ou cria o seu próprio padrão para estabelecer este critério, o que torna muito difícil a padronização de códigos infravermelhos entre os equipamentos.
Exemplo de “marca” e “espaço”.

<img src="/imagens/2SB3IRRF.png" height="200" witdh="20">

O módulo SB3IRRF utiliza o conceito de HEXCODE ou código reduzido para a transmissão de códigos de infravermelho para cada fabricante, marca e modelo.

Uma vez cadastrados nos módulos os parâmetros de envio relativos a: frequência, tamanho do código, repetições, tempos de “marca” e “espaço” para início (Lead in), fim (Lead out), “1”-s (Burst 1) e “0”-s (Burst 0),  para um determinado modelo, basta enviar o código propriamente dito, também chamado de HEXCODE para que o módulo SB3IRRF atue no equipamento. Desta forma o tamanho do código enviado fica bastante reduzido, permitindo que pulsadores sem fio, enviem códigos para ligar, desligar ou operar equipamentos. 

<img src="/imagens/i.png" height="40" witdh="40">  Informações| Informações!
------------ | -------------
  * |É possível alterar a configuração de fábrica através do computador utilizando o adaptador para porta USB que é vendido separadamente ou através de outro equipamento ligado na mesma (NET ID).
  * | Para utilizar a comunicação com o computador é necessário além do adaptador para porta USB, a instalação do programa de comunicação com portas Seriais. A configuração da porta serial deve ser: 57600, N, 8, 1.
  * | Acesse http://www.wtihome.com.br/suporte para mais informações.

##4. Comunicando o Equipamento com Outros Módulos

É possível associar vários equipamentos do sistema @home permitindo criar uma rede de equipamentos, cujo principal objetivo é criar cenários complexos e ampliar o alcance da rede. Esta associação pode ser feita mesmo sem a necessidade da central Net Center:

1. Configure cada um dos equipamentos com um endereço diferente mas na mesma (NET ID) para que seja possível que os equipamentos interajam entre si.

2. Posicione os equipamentos de tal forma que nenhum equipamento fique fora do alcance de pelo menos um dos equipamentos que se deseja interligar.

3. Altere os cenários pré-determinados para realizar as cenas desejadas.

<img src="/imagens/i.png" height="40" witdh="40">  Informações| Informações!
------------ | -------------
  * | É possível alterar a maioria das funções de controle e comando dos equipamentos @home sem a necessidade da central Net Center.
  * | É possível configurar todas as funções dos equipamentos através do computador e do adaptador USB.
  * | A central Net Center é necessária quando se deseja controlar os equipamentos através de smartphones ou tablets ou executar cenas em horários pré-determinados.

##5. Cénarios

O módulo SB3IRRF pode armazenar até 20 cenários diferentes em dois bancos de cenários, chamados: “Banco S” e “Banco T”. Os cenários são chamados S0 a S9 e T0 a T9 e podem ser executados através de outros equipamentos ligados na rede @home.

<img src="/imagens/i.png" height="40" witdh="40">  Informações| Informações!
------------ | -------------
  * |Cada cenário pode armazenar um máximo de 24 caracteres. Como um comando básico possui de 3 a 5 caracteres, cada cenário pode armazenar de 5 a 8 comandos. Cada comando deve ser separado pelo caractere “;”. É possível encadear cenários, aumentando consideravelmente a quantidade de comandos executados por vez.

Exemplo de cenários:

**“R1 1 04FBC43B”** - Desliga uma TV LG pela porta 1  
**“S0”** - Executa o cenário S0  
**“30:L1”** - Envia para o equipamento cujo endereço é 30, o comando “L1”  

##6. Comandos 

Os seguintes comandos estão disponíveis no módulo SB3IRRF podendo ser enviados através de outros equipamentos, como também da central Net Center.

Se os comandos forem enviados através do conector de programação, ao final de cada grupo de comandos deve ser enviado o caractere LF  (Line Feed)

######Os comandos seguem o formato:

Comando parametro1 parametro2 parametro3 parametro4 onde os parâmetros podem ser opcionais dependendo do tipo de comando.

Para enviar comandos para outros equipamentos, deve-se informar o endereço do equipamento destino, sempre com 2 caracteres, seguido do caractere “:” antes do comando a ser enviado:

######Exemplo:
**“30:L1”** - Envia para o equipamento cujo endereço é 30, o comando “L1”. 

**Grupo 1 – Comandos para  ligar/desligar as lâmpadas**

R1, R2 ou R3| Envia um comando infravermelho para a porta 1, 2 ou 3 respectivamente.
------------ | -------------
**Parâmetros disponíveis**|
type|Identificador que contém os parâmetros necessários para converter o HEXCODE no código completo a ser enviado para o equipamento. Os parâmetros devem ter sido previamente cadastrados através dos comentos: IR, IL, IB e SV.
bits (opcional)|Tamanho em bits do dado a ser enviado). Determinados equipamentos possuem tamanhos de códigos diferentes para comandos diferentes. Neste caso é possível informar o tamanho do código que deve ser enviado. Se este parâmetro não for informado, o módulo tentará calcular a quantidade de bits através do tamanho do hex code informado.
Hex code|Dado a ser enviado ao equipamento, também chamado de HEXCODE. Caso este parâmetro não seja informado o dado que será utilizado para envio virá do “buffer” interno que foi alimentado previamente através dos comandos: D1, D2, D3 e D4.

D1, D2, D3 ou D4|Alimenta o “buffer” interno de envio com o HEXCODE para posterior utilização pelos comandos R1, R2 ou R3.
------------ | -------------
tamanho|O tamanho máximo do comando que o módulo SB3IRRF pode enviar tem 23 posições. As vezes um código infravermelho mesmo utilizando-se o seu hex code é  maior que isso. Neste caso o hex code precisa ser quebrado em vários pedaços, armazenados em um “buffer” interno, para posterior envio.
quantidade|Existem 4 “buffers” que podem ser alimentados com pedaços do hex code e que são unidos novamente na no momento do envio.
**Parâmetros disponíveis**|
dado|Valor em hexadecimal a ser inserido no buffer de envio.
Exemplo|Suponha o seguinte hex code cujos parâmetros de envio estão cadastrados com o identificador 10: 0102030405060708090A0B0C0D0E0F1011 Envio local (*) D1 0102030405060708090A   D2 0B0C0D0E0F1011  R1 10 Envio remoto (*)  30:D1  0102030405060708  30:D2 090A0B0C0D0E0F10  30:D3 11  R1 10 
**(*)**|**Observe que em ambos os casos o tamanho total da linha de comando não pode ultrapassar 23 caracteres.**
LR |Recebe um novo comando Infravermelho através de um controle remoto existente. Ao se digitar este comando o módulo SB3IRRF entra no modo de “learning” no qual ficará aguardando um comando IR através da sua entrada de captura na parte de cima do equipamento. Caso um comando válido seja recebido, este será enviado para a porta de comunicação do equipamento. A porta de comunicação poderá ser ligada a um computador através de adaptador para porta USB (vendido separadamente). Uma vez recebido pelo computador este comando poderá ser convertido para um HEXCODE.
IR, IL, IB, SV e LD|Cria ou altera um novo conjunto de parâmetros de um determinado fabricante, marca e modelo que serão utilizados na hora de expandir um hex code. 

IR|Cria um novo conjunto de parâmetros em memória
------------ | -------------
**Parâmetros disponíveis**|
type |Identificador deste conjunto de parâmetros que seár utilizado posteriormente nos comandos: R1, R2 e R3. 
Khz | Frequência de envio dos códigos em kHz.
bits |Quantidade de bits padrões que é esperada no hex code. Esta informação pode ser sobreposta no momento do envio, caso contrário esta será utilizada.
repeat |Quantidade de repetições que o hex code será enviado.

IL|Altera os tempos e a ordem em que são enviados as “marcas” ou “espaços” no início ou final da transmissão.
------------ | -------------
**Parâmetros disponíveis**|
begin1|pulsos de “marca” ou “espaço” no início 
begin2|pulsos de “marca” ou “espaço” no início 
end1|pulsos de “marca” ou “espaço” no início 
end2| pulsos de “marca” ou “espaço” no início
**(*)**|**Números positivos representam “marcas” e números negativos representam “espaços”.**
**(**)**|**O tempo efetivo em microssegundos da “marca” ou “espaço” pode ser obtido multiplicando-se os pulsos por 1000 (mil) e dividindo pela frequência: **Exemplo: IL 190 -250 * (5000 microssegundos de marca e 6578 microssegundo espaço)**

IB| Altera os tempos e a ordem em que são enviados as “marcas” ou “espaços” no bit “1” e do bit “0”.
------------ | -------------
**Parâmetros disponíveis**|
bitone1|pulsos de “marca” ou “espaço” do bit 1
bitone2|pulsos de “marca” ou “espaço” do  bit 1
bitzero1|pulsos de “marca” ou “espaço” do bit 0 
bitzero2|pulsos de “marca” ou “espaço” do bit 0
**(*)**|**Números positivos representam “marcas” e números negativos representam “espaços”.**
**(**)**| O tempo efetivo em microssegundos da “marca” ou “espaço” pode ser obtido multiplicando-se os pulsos por 1000 (mil) e dividindo pela frequência:Exemplo: IL 190 -250 * (5000 microssegundos de marca e 6578 microssegundos espaço)**

SV|Salva os parâmetros configurados em memória em uma das 10 posições disponíveis (0 a 9)
------------ | -------------
**Parâmetros disponíveis**|
pos | Posição a salvar o novo conjunto de parâmetros 
LD |Carrega parâmetros salvos anteriormente para a memória. Geralmente para edição.
**Parâmetros disponíveis**|
pos |Posição da qual carregar  os parâmetros

**Grupo 2 – Comandos gerais de configuração do rádio e da rede**

$RAD|Endereço e outros parâmetros do rádio NRFWTI
------------ | -------------
**Parâmetros disponíveis**|
endereço |Endereço único na rede, no formato hexadecimal (Default: 88 – valores entre 00 e FE). (*)
Frequência RF |Variação em 1Mhz da frequência de operação do rádio no intervalo de 2400Mhz a 2525Mhz, seguindo a fórmula: 2400 + Frequência RF |(Default: 76 – valores entre 0 e 125).
Roteador|Ativa ou desativa a função de roteador, que faz com que o rádio retransmita pacotes dentro da rede: (Default: 0).
0|Não funciona como roteador
1 |Funciona como roteador
Somente Transmite| Liga ou desliga o modo de recepção do rádio: (Default: 0)
0|Transmite e recebe
1 | Somente Transmite

$NET |NET ID e endereço da Central Net Center (*)
------------ | -------------
**Parâmetros disponíveis**|
central|Endereço único da central Net Center, no formato hexadecimal.(Default: FF – valores entre 00 e FF)
offset1|Primeiro byte do NET ID, no formato hexadecimal (Default: 3C – valores entre 00 e FF) 
offset2|Segundo byte do NET ID, no formato hexadecimal (Default: 5A – valores entre 00 e FF)
offset3|Terceiro byte do NET ID, no formato hexadecimal (Default: 69 – valores entre 00 e FF) 
**(*)**|**O endereço NET ID é formado por 3 bytes e deve ser igual para todos os equipamentos de uma mesma rede. Mesmo que outra rede esteja na mesma frequência de rádio, o NET ID vai garantir que haja uma independência entre elas. NUNCA DEIXE SEU NET ID COM OS PADRÕES DE FÁBRICA**

$PAR|Parâmetros de transmissão do rádio.
------------ | -------------
**Parâmetros disponíveis**|
Potência | Potência de transmissão (Default: 3)
0 |– Mínima
1 |Média
2 |Alta
3 | Máxima
Velocidade |Velocidade de transmissão  (Default: 2)
0 |1Mbps
1 | 2Mbps
3 | 250Kbps
Tamanho CRC| Quantos bytes ocupa o CRC “Controle de Checagem de Erro” em cada pacote transmitido (Default: 2)
0 |Desabilitado
1 | 8bits
2 | 16bits

$RET|Parâmetros de retransmissão do rádio.
------------ | -------------
**Parâmetros disponíveis**|
Atraso |Atraso entre as retransmissões, em múltiplos de 4ms, no caso de falha (Default: 4, valores entre 0 e 15)
Quantidade|Quantidade de retransmissões (Default: 4, - valores entre 0 e 15)

$NEA|Endereço dos equipamentos próximos desabilitando-se assim a função autodiscover.
------------ | -------------
**Parâmetros disponíveis**|
endereço1 a 4 | Endereço de um equipamento próximo , no formato hexadecimal (Default: FF – valores entre 00 e FF) (*)
**(*)**| O endereço FF não é associado a nenhum equipamento e deve ser utilizado quando se deseja retornar ao modo autodiscover: $NEA FF FF FF FF.**

<img src="/imagens/i.png" height="40" witdh="40">  Informações| Dicas para Configuração
------------ | -------------
*|A maioria dos comandos de configuração do rádio e da rede já vem pré-definidos de fábrica para seu melhor desempenho. Não é necessário nenhum ajuste adicional.
*|O endereço do rádio, o NET ID e o canal do rádio por estarem com seus parâmetros default, devem ser alterados para evitar interferência com outros equipamentos ou outras redes. Comandos $RAD e $NET.
*|Pode-se usar o caractere “?” quando não se deseja alterar o valor de um determinado parâmetro:
Ex: $RAD ? 77| O endereço do rádio permanece inalterado, e a frequência do rádio foi alterado para o canal 77. 
*|Após qualquer alterações nas configurações é necessário salvá-las e reinicializar o equipamento para que as mesmas surtam efeito. Utilize $SAV e $RST respectivamente.

**Grupo 3 – Outros comandos gerais**

$SAV| Salva os parâmetros configurados na memória não volátil (EEPROM)
------------ | -------------
$STA |Envia os parâmetros configurados para a porta de configuração caso o comando tenha sido recebido por ela, ou para o equipamento requisitante. 
$SCE| Envia os cenários cadastrados para a porta de configuração caso o comando tenha sido recebido por ela, ou para o equipamento requisitante caso tenha havido a solicitação de um cenário específico. 
**Parâmetros disponíveis**|
banco |Número do banco que se deseja mostrar. (Default: todos – valores 1, 2 ou 3 para os bancos A, B e S respectivamente).
cenário|Número do cenário que se deseja mostrar dentro do banco especificado. (Default: 0 – valores 0 até o total de cenários do banco) (*).Ao final dos cenários também são mostrados os parâmetros de configuração de envio de IR cadastrados.
$FDF |Retorna todos os parâmetros do equipamento para os ajustes de fábrica e executa um reset geral.
$VER|Envia a versão de firmware para a porta de configuração caso o comando tenha sido recebido por ela, ou para o equipamento requisitante.
$RST|Reinicia o equipamento

**Grupo 4 – Comandos para cenários**

Executa o respectivo cenário |S0,S1,S2,S3,S4,S5,S6,S7,S8 e S9, T0,T1,T2,T3,T4,T5,T6,T7,T8 e T9 
------------ | -------------
Grava o respectivo cenário|WS0,WS1,WS2,WS3,WS4,WS5,WS6,WS7,WS8,WS9,WT1,WT2,WT3,WT4,WT5,WT6,WT7,WT8,WT9
**Parâmetros disponíveis**|
Comandos | Comandos que serão executados pelo cenário específico. Caso seja necessário a execução de mais de um comando, é necessário separar cada comando pelo caractere “;” e o colocar o conjunto inteiro entre aspas duplas: Ex: WS0 R1 10 14231215

##7. Procedimentos para Mau Funcionamento

O equipamento não responde a uma transmissão remota:

  * Verifique se o alcance máximo não foi excedido e que o sinal não está obstruído por superfícies ou caixas de metal. O led ACT pisca em intervalos constantes, mas quando um comando válido é recebido a frequência da piscada muda por alguns segundos. Verifique se o módulo está recebendo comandos corretamente através da visualização do led ACT.

  * Caso o equipamento tenha sido reiniciado recentemente, envie alguns comando adicionais para que a memória dos equipamentos remotos limpe qualquer referência de informação deste equipamento. 

##8. Ajustes de Fábrica
Caso necessário, é possível ajustar o equipamento para os padrões de fábrica. Insira um objeto pontiagudo no orifício situado ao lado do conector de programação, exercendo uma leve pressão. Aguarde 5 segundos com o objeto inserido e verifique se o led ACT ficou aceso por 2 segundos. O equipamento ira resetar com os parâmetros de fábrica configurados. 

##9. Garantia

######I - Prazo e Comprovação da Garantia

  * O produto abaixo identificado, devidamente lacrado, é garantido pelo seu fabricante e/ou importador (XSOLUTIONS S.A.), pelo prazo de um ano, contado a partir da data de sua aquisição pelo primeiro consumidor e obedecidas as condições e as recomendações especiais aqui discriminadas.

  * Esta garantia contratual é dada ao produto abaixo identificado, exclusivamente contra eventuais defeitos decorrentes de projeto, fabricação, montagem, ou quaisquer outros vícios de qualidade que o tornem impróprio ou inadequado ao uso regular.

  *  Para a comprovação desse prazo, o consumidor deverá apresentar este Termo de Garantia, devidamente preenchido, e/ou a 1ª via da nota fiscal de compra, ou outro documento fiscal equivalente, desde que identifique o produto.
Exija do estabelecimento comercial revendedor, o preenchimento correto deste Termo de Garantia.

######II- Exclusão da Garantia

A garantia não abrangerá, sendo, pois, ônus do consumidor:

a) Os danos sofridos pelo produto, ou seus acessórios, em consequência de acidente, maus tratos, manuseio ou uso incorreto e inadequado;

b) Os danos sofridos pelo produto, em consequência de sua utilização para finalidades diversas das especificadas pelo fabricante e/ou importador (XSOLUTIONS S.A.), ou incompatíveis com a destinação do mesmo.

######III- Local Onde a Garantia Deverá ser Exercitada

  * Os consertos em garantia somente deverão ser efetuados por uma Assistência Autorizada, devidamente nomeada pelo fabricante e/ou importador (XSOLUTIONS S.A.), que, para tanto, se utilizará de técnicos especializados e de peças originais, relacrando o seu aparelho e garantindo o serviço executado.

######IV- Cessação da Garantia

  *  Não confie o conserto do produto abaixo identificado a curiosos, pessoas ou oficinas não autorizadas e não credenciadas pelo seu fabricante e/ou importador (XSOLUTIONS S.A.).

  *  Se isto vier a ocorrer, com a consequente violação do lacre do produto, a garantia cessará, de imediato.

  * O produto abaixo identificado foi projetado para funcionamento em uso doméstico, única e exclusivamente. A sua utilização, para uso não doméstico, industrial ou comercial, acarretará a cessação imediata da garantia.


######V- Recomendações Especiais

  * Antes de colocar o produto em funcionamento, leia atentamente as instruções de uso e/ou instalação contidas no próprio aparelho, na embalagem, ou no manual respectivo. Siga-as rigorosamente. Elas são a sua segurança.

  * Certifique-se de que a voltagem a ser utilizada é a mesma indicada no aparelho (110V a 220V). Verifique se a instalação elétrica do local está correta e adquada.

  * Para evitar danos, mantenha o produto bem armazenado e limpo, em ambiente protegido das intempéries (chuva, vento, umidade, raios solares, etc.).

  * Não introduza quaisquer objetos estranhos à função própria do produto, principalmente quando este estiver em funcionamento, evitando acidentes.

######VI - Fabricante e/ou Importador

XSOLUTIONS S.A.  
CNPJ/M.F. Nº 61.064.978/0001-01  
Av. Carlos Vasconcelos, 1702 – Aldeota – Fortaleza/CE

Qualquer reclamação, comentário ou sugestão sobre o atendimento e os reparos prestados pelas Assistências Autorizadas, ligue ao nosso Serviço de Atendimento ao Consumidor.

Departamento de Assistência Técnica:(85) 3311.6464.
