# NetCenter

A Central de Automação @home é um gateway que interliga todos os módulos instalados com a rede WiFi. Sua topologia sem fio permite comunicação rápida e eficaz entre os módulos, independente do seu local de instalação. A Central permite que todas as funcionalidades da linha @home sejam acessadas através de smartphones, tables e notebooks, assim como o agendamento de tarefas, a programação de cenários e o acesso remoto. 
Promove a interação com diversos tipos de sensores, proporciona total integração com equipamentos multimídias. Além de permitir o controle e dimerização personalizadas de lâmpadas ou leds.

1. [Instalação](#instalação)
2. [Configuração Inicial](#configuração)
   * [Conexão através da interface web](#conexão-através-da-interface-web)
   * [Conexão através de um computador interligado](#conexão-através-de-um-computador-interligado)
   * [Conexão através de um teclado USB e monitor HDMI](#conexão-através-de-um-teclado-usb-e-monitor-hdmi)
   * [Interface de linha de comandos](#interface-de-linha-de-comandos)
3. [Interface Web](#interface-web)
   * [Ambientes](#ambientes)
   * [Categorias](#categorias)
   * [Cenas](#cenas)
   * [Eficiência Energética](#user-contente-eficiencia-energetica)
   * [Eficiência Térmica](#user-contente-eficiencia-termica)
   * [Administração](#administração)
       * [Ambientes](#user-content-administracao-ambientes)
       * [Módulos](#user-content-administracao-modulos)
       * [Categorias](#user-content-administracao-categorias)
       * [Dispositivos](#user-content-administracao-dispositivos)
       * [Entradas](#user-content-administracao-entradas)
       * [Serviços](#user-content-administracao-servicos)
       * [Comandos](#user-content-administracao-comandos)
       * [Cenas](#user-content-administracao-cenas)
       * [Tarefas](#user-content-administracao-tarefas)
       * [Usuários](#user-content-administracao-usuarios)
       * [LayOuts](#user-content-administracao-layouts)
       * [Comandos de Voz](#user-content-administracao-voz)
         * [Lista de Comandos](#user-content-administracao-voz-comandos)
         * [Palavras a Descartar](#user-content-administracao-voz-descartar)
   * [Configuração](#configuração)

## Instalação

A central NetCenter pode ser instalada em qualquer lugar que seja possível a interligação com pelo menos
um módulo da tecnologia atHome. Ela é totalmente sem fio, e só precisa estar ligada à rede elétrica.

## Configuração Inicial

> A Central NetCenter após inicializada,  publica seu próprio nome na rede interna via mDns 
> para um acesso mais fácil. O nome padrão para acesso é ```athome.local```. O protocolo mDns não está
> disponível em todos os sistemas operacionais. Caso não seja possível acessar a Central NetCenter pelo
> nome, utilize o endereço IP configurado abaixo.

A Central NetCenter disponibiliza uma interface Web para a sua operação e configuração, além de uma interface de linha de comandos, assim como o acesso via monitor HDMI e teclado via porta USB.

Para acessar esta interface, utilize uma das formas descritas abaixo:

### Conexão através da interface Web

A Central NetCenter vem programada de fábrica para habilitar um ponto de acesso Wi-Fi chamado "NetCenter".
É possível se conectar a este ponto de acesso e configurar a interface a partir deste.

* Ligue a Central NetCenter na tomada e aguarde 30 segundos.
* Através de um computador ou smartphone, procure pelo ponto de acesso "NetCenter" e conecte-se com ele (Não precisa de senha)
* A Central NetCenter vem configurada de fábrica no endereço IP 192.168.3.2
* Utilize qualquer navegador e acesse o endereço http://192.168.3.2

```
login: admin@home.com
password: 1234
```

### Conexão através de um computador interligado

Interligue um computador com a Central NetCenter através do cabo de rede fornecido
junto com o equipamento.

* Ligue a Central NetCenter na tomada e aguarde 30 segundos.
* Conecte o cabo de rede na Central NetCenter e no computador que será usado na configuração
* A Central NetCenter vem configurada de fábrica no endereço IP 192.168.2.2, configure o  endereço IP 
do computador para 192.168.2.1/255.255.255.0 para ter acesso à Central.
* Utilize qualquer programa que utilize o protocolo ssh, tal como "putty", ou "ssh".
* Conecte-se via SSH ao endereço da Central NetCenter

```
login: console
password: admin
```

### Conexão através de um teclado USB e monitor HDMI
Conecte um teclado e um monitor 

* Conecte um teclado USB a uma das duas portas USB na parte frontal do equipamento
* Conecte um cabo HDMI na parte traseira do equipamento interligado a um monitor/TV
* Ligue a Central NetCenter na tomada e aguarde 30 segundos.
* Caso esteja aparecendo no monitor o símbolo da @home, pressione ```alt+F2```

```
login: console
password: admin
```

### Interface de linha de comandos

A interface de linha de comandos é utilizada para configurar diversos parâmetros da Central NetCenter. 
A lista de comandos disponibilizada pode ser visualizada através do comando ```help```

```
atHome> help
atHome> help show
atHome> help show network
```
#### Visualizar interfaces de rede
```
atHome> show network status
```
>A Central NetCenter possui duas interfaces de rede. Uma cabeada localizada na parte traseira do equipamento,
>chamada de *lan* e outra wireless embutida chamada de *wlan*.

#### Habilitar a interface cabeada
```
atHome> set lan mode enabled
```
#### Configurar a interface cabeada para DHCP
```
atHome> set lan mode dhcp
```
>Recomenda-se utilizar a Central NetCenter no modo DHCP e reservar um endereço IP no roteador 
>da residência, através do *MAC address* que pode ser obtido pelo comando ```show network status```.

#### Configurar a interface cabeada para endereço estático
```
atHome> set lan mode static
atHome> set lan address 192.168.2.2
atHome> set lan mask 255.255.255.0
```
#### Habilitar a interface wireless
```
atHome> set wlan mode enabled
```
#### Configurar a interface wireless para DHCP
```
atHome> set wlan mode dhcp
```
#### Configurar o *access point* da interface wireless
```
atHome> set wlan ssid "MINHA REDE"
atHome> set wlan ssid "senhasenha"
```
#### Verificar se existe uma nova atualização de software
```
atHome> version check
```
#### Atualizar para uma nova versão de software
```
atHome> version update
```
#### Reiniciar o equipamento
```
atHome> reboot
```
>Algumas alterações nas interfaces de rede só surtem efeito após a reinicialização da Central NetCenter.

## Interface Web

Após a configuração inicial da Central NetCenter é possível acessá-la via interface Web através do
endereço ```http://athome.local``` ou ```http:endereco_ip_configurado```. A primeira tela disponibilizada
é a tela de login.
```
login: admin@home.com
senha: 1234
```
A tela da interface Web é dividida em:
* Uma área para envio de comandos na parte superior
* Uma área para de menu lateral do lado esquerdo
* Uma área de operação ao centro

### Ambientes
Serão visualizados todos os ambientes criados no menu **Administração | Ambientes**, e uma vez clicados 
trarão todos os dispositivos disponíveis para aquele ambiente específico, com sua respectiva tela de operação. 
>A tela de operação de cada dispositivo depende do tipo de dispositivo. Sempre será possível visualizar o nome do
>dispositivo, seu ícone e uma seta para baixo, que uma vez clicada, mostrará as opções adicionais de 
>operação deste dispositivo, como por exemplo: controles de dimerização, controle de ar-condicionados, etc.

>ESTA É A TELA PADRÃO DO SISTEMA APÓS O LOGIN

### Categorias
Serão visualizadas todas as categorias criadas no menu **Administração | Categorias**, e uma vez clicadas
trarão todos os ambientes que possuem dispositivos na categoria selecionado. A partir daí a utilização é idêntica
como se tivesse clicado em **Ambientes**.

### Cenas
Serão visualiadas todas as cenas criadas no menu **Administração | Cenas** e uma vez clicadas iniciarão
imediatamente a execução da referida cena.

### Administração
Este menu só é disponibilizado se o usuário conectado possuir permissões de administrador, caso contrário, 
somente os três menus acima estarão disponíveis. É neste menu que serão administrados todos os itens que
compõem o ecossitema NetCenter tais como: ambientes, categorias, cenas, tarefas agendadas, etc.

<a name="administracao-ambientes"></a>
#### Ambientes
Os ambientes são agrupamentos de dispositivos baseados em sua localização física. Geralmente os 
ambientes dizem respeito aos cômodos de uma residência ou locais específicos. Posteriormente na administração
de dispositivos será possível atribuir um dispositivo em um ou mais ambientes.

Exemplos: Sala de Estar, Sala de Jantar, Cozinha, etc.

>O campo **sequência** será utilizado na tela de **Ambientes** para ordenação. Caso
>hajam ambientes com a mesma sequência a ordem alfabética será utilizada, para a mesma sequência.

<a name="administracao-categorias"></a>
#### Categorias
As categorias são agrupamentos de dispositivos baseados em alguma característica. Geralmente as 
categorias dizem respeito ao tipo de dispositivo. Posteriormente na administração
de dispositivos será possível atribuir um dispositivo a uma ou mais categorias..

Exemplos: Iluminação, Multimídia, Refrigeração, etc.

>O campo **sequência** será utilizado na tela de **Ambientes** para ordenação. Caso
>hajam ambientes com a mesma sequência a ordem alfabética será utilizada, para a mesma sequência.

<a name="administracao-modulos"></a>
#### Módulos
Os módulos são os equipamentos de atuação e/ou controle que serão utilizados para formar o projeto
de automação. Podem ser equipamentos da WTI@home, como o B3R3PRF, SB3IRRF,  ou de outros fabricantes. 
Cada módulo adquirido deve ser inserido neste menu, com as suas respectivas características. 
Há uma relação direta entre módulos e dispositivos, pois cada módulo disponibiliza uma ou mais 
portas de atuação. Cada porta de atuação será atribuída a um dispositivo no momento do seu cadastro.

Exemplo: O módulo de relés B3R3PRF disponibilizará 3 portas, uma para cada circuito a ser controlado

>O campo **endereço** representa o endereço do módulo da WTI@home dentro do projeto. Ele deve ser inserido
>no formato hexadecimal, com 2 posições e ser único. Obviamente o módulo físico deve ter sido configurado 
>com este mesmo endereço haja visto que este será o destino das mensagens de atuaçao que serão enviadas para 
>cada dispositivo que esteja a atrelado a este módulo.
>
>Exemplos: 01, 20, 22, 35

>O campo **versão** indica a versão do firmware do módulo. Ao cadastrar o módulo, automaticamente a central
>enviará um comando a este solicitando sua versão de firmware. Caso não seja possível obtê-la será mostrado
>um botão com o texto **Obter**, neste caso basta clicá-lo para que a central envie novamente o comando de
>solicitação para o módulo. Caso exista uma versão de firmware do módulo mais recente que a versão instalada
>isto será indicada por um outro botão ao lado da versão atual, com o número da versão mais recente. Para
>atualizar para esta versão, basta clicar neste botão e responder **Sim** para a pergunta de confirmação.
>A partir daí será iniciada o envio em segundo plano do novo firmware para o respectivo módulo,
>que poderá ser acompanhada através do percentual de conclusão que será mostrado.
>O fim da atualização ser indicado por um botão com o texto **Reboot**, indicando que a atualização já foi
>enviada e que o módulo está pronto para atualização, bastando para isso clicá-lo e responder **Sim** para a
>pergunta de confirmação. Caso o novo firmware não consiga ser enviado para o módulo, isto será indicado através
>de um botão com o texto **Erro**. Ao clicá-lo o campo voltará a mostrar a versão atual.

<a name="administracao-dispositivos"></a>
#### Dispositivos
Os dispositivos são os equipamentos que se deseja controlar, tais como: lâmpadas, fitas led, TVs, ar-condicionados, etc.
Cada dispositivo estará associado a uma porta de um módulo previamente cadastrado. Após o cadastro o dispositivo
será visualizado no ambiente ou ambientes aos quais foi associado.

>O campo **porta** refere-se a porta livre de um determinado módulo ao qual este dispositivo está conectado ou será
>controlado. Para cada dispositivo cadastrado a porta referente aquele dispositivo não aparecerá mais na lista de
>portas disponíveis.

>O campo **nome** é utilizado para referenciar este dispositivo nos cenários, entradas, tarefas ou entrada de
>linha de comando. Deve começar com letras e só possuir letras, números ou o caractere "_"
>
> Exemplo: **LP_LAMPADA_01** ou **IR_TV_01**
>

##### Dispositivos do módulo [SB3R3PRF](#/documentacao/SB3IRRF.md)
Ao se cadastrar um dispositivo referente a uma porta do módulo **SB3IRRF** (Módulo de InfraVermelho) alguns
parâmetros adicionais estarão disponíveis, tais como: Tipo, Marca e Modelo. Estes parâmetros serão utilizados
pela Central NetCenter para um correto envio do comando IR (InfraVermelho) correto para o equipamento. **Caso
a marca ou modelo selecionado não esteja disponível na lista, será possível capturar os códigos a partir do
controle remoto e enviá-los à WTI para inclusão. Verificar na documentação do módulo
[SB3IRRF](#/documentacao/SB3IRRF.md)**. Após incluir o dispositivo, é necessário enviar a configuração desta 
marca/modelo para o módulo físico para que os comandos enviados, reflitam o equipamento correto. Para isso 
na entrada da linha de comando digite:

```
REMOTE nome_do_dispositivo CONFIG
```
substitindo **nome_do_dispositivo** pelo **nome** utilizado para referenciar o dispositivo.

<a name="administracao-entradas"></a>
#### Entradas

Uma entrada é um nome que damos para um comando a ser executado na Central NetCenter. Isso permite que
qualquer módulo que componha a rede atHome envie uma entrada para a
Central NetCenter. Uma aplicação prática seria através de um pulsador solicitar a execução de um cenário complexo:

Exemplo:

- Supondo que o endereço da Central NetCenter seja **30**
- Programar no pulsador o envio do comando **30:TESTE**
- Criar a entrada **TESTE** na Central NetCenter
- Atribuir a entrada **TESTE** para o comando específico: **play cenario_qualquer**
- Ao apertar o pulsador, a Central NetCenter executará o cenário **cenario_qualquer**

>O campo **nome** é utilizado como identificador desta entrada.  
>Deve começar com letras e só possuir letras, números ou o caractere "_"
>
> Exemplo: **LP_LAMPADA_01** ou **IR_TV_01**
>

##### Comandos do módulo [B433RF](#/documentacao/B433RF.md)
O módulo **B433RF** após aprender um novo código na frequência de 433Mhz, e estando com o endereço da Central
NetCenter configurado, fará o envio deste código RF433Mhz para a Central NetCenter, que irá cadastrá-lo 
automaticamente como uma nova entrada, cabendo ao administrador informar qual comando específico deve ser executado. 
Desta forma, sempre que este código RF433Mhz for recebido pelo módulog **B3433RF**, a Central NetCenter 
irá executar o comando atribuído a esta entrada.

Este código geralmente é no fomato: RF433_**AABBCC** onde **AABBCC**, representam um código único para cada 
código aprendido. 

> Verificar nos exemplos de cenário a [Central de Alarme](#cenarios/CENTRAL_ALARME.md)

<a name="administracao-servicos"></a>
#### Serviços

A central NetCenter é composta por vários serviços. Cada serviço é responsável por uma atividade dentro da Central. Por exemplo: O serviço **TASKS** é responsável pelas tarefas agendadas, o serviço **WEB** é responsável por disponibilizar a interface Web e assim sucessivamente. Desta forma é possível cadastrar novos serviços, sejam eles interfaces com outros fabricantes ou interligar centrais NetCenters para a execução de tarefas cooperativas.

<a name="administracao-comandos"></a>
#### Comandos

Cada comando executam tarefas expecíficas dentro das cenas. Você pode visualizar cada um dos comandos que podem ser usados nos cenários, sua descrição, forma de uso e exemplos para explorar toda a potencialidade da central NetCenter.

<a name="administracao-tarefas"></a>
#### Tarefas

Uma tarefa é um [comando](#user-content-administracao-comandos) que você deseja executar posteriormente, seja de forma repetitiva em intervalos regulares, seja respeitando uma agenda, ou uma única vez no futuro. 

Existem 3 tipos de agendamento para tarefas:

##### Agenda

Uma agenda é um tipo de tarefa que é executada periodicamente em qualquer intervalo de tempo pré-determinado. Ela possui uma grande flexibilidade, pois permite utilizar datas e horas específicas em sua composição.

Para cada um dos campos, preencha quando necessário os intervalos utilizando o separador "-" ou valores específicos utilizando o separador "," ou ambos. Por exemplo: 1,2,5-8,10. Se o campo não estiver preenchido, significa que este campo não será utilizado para o cálculo do intervalo.

Exemplo:

```
Comando : play cena_exemplo
Horas   : 10-12,18,20
Minutos : 0,30
```

Nesta caso o comando **play cena_exemplo** será executado as 10h00m, 10h30m, 11h00m, 11h30m, 12h00m, 12h30m, 18h00m, 18h30m, 20h00, 20h30m

##### Intervalo

Um intervalo é um tipo de tarefa que é executada a cada intervalo de tempo pré-determinado, tendo sempre como base a data inicial da tarefa.

Ela é extremamente útil quando se deseja executar uma tarefa com a mesma recorrência independente de sua data e hora. Considere cada período de tempo como um "a cada 'n' períodos".

Diferentemente do tipo agenda, um valor de horas igual a 3, não irá executar uma tarefa às 03 horas da manhã, mas a **cada** 3 horas.

```
Comando : play cena_exemplo
Horas   : 3
Minutos : 30
```

O comando **play cena_exemplo** será executado a cada 3 horas e 30 minutos.

##### Uma Vez

Este tipo de agendamento é utilizado quando se deseja executar um comando uma única vez em uma data futura.

<a name="administracao-usuarios"></a>
#### Usuários

A central NetCenter pode ser utilizada por vários usuários simultaneamente e independentemente. É aqui que é realizado o cadastro dos usuários que poderão utilizá-la, seja via interface Web ou via aplicativo mobile, assim como se os mesmos são administradores ou somente usuários.

**O menu Administração e o menu Configuração só aparecem caso o usuário esteja marcado como Administrador**.

<a name="administracao-layouts"></a>
#### LayOut

Um "layout" representa um desenho de tela de um novo dispositivo, geralmente controles remotos, com seus respectivos botões para que possam ser programadas as funções em cada um deles. O formato padrão do "layout" é o formado JSON. Após a inclusão de um layout, o mesmo poderá ser utilizado quando da criação de dispositivos virtuais.
