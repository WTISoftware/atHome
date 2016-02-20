# NetCenter

A Central de Automação @home é um gateway que interliga todos os módulos instalados com a rede WiFi. Sua topologia sem fio permite comunicação rápida e eficaz entre os módulos, independente do seu local de instalação. A Central permite que todas as funcionalidades da linha @home sejam acessadas através de smartphones, tables e notebooks, assim como o agendamento de tarefas, a programação de cenários e o acesso remoto. 
Promove a interação com diversos tipos de sensores, proporciona total integração com equipamentos multimídias. Além de permitir o controle e dimerização personalizadas de lâmpadas ou leds.

1. [Instalação](#instalação)
2. [Configuração Inicial](#configuração)
   * [Conexão através de um computador interligado](#conexão-através-de-um-computador-interligado)
   * [Conexão através de um teclado USB e monitor HDMI](#conexão-através-de-um-teclado-usb-e-monitor-hdmi)
   * [Interface de linha de comandos](#interface-de-linha-de-comandos)
3. [Interface Web](#interface-web)

## Instalação

A central NetCenter pode ser instalada em qualquer lugar que seja possível a interligação com pelo menos
um módulo da tecnologia atHome. Ela é totalmente sem fio, e só precisa estar ligada à rede elétrica.

## Configuração Inicial

> A Central NetCenter após inicializada,  publica seu próprio nome na rede interna via mDns 
> para um acesso mais fácil. O nome padrão para acesso é ```athome.local```. O protocolo mDns não está
> disponível em todos os sistemas operacionais. Caso não seja possível acessar a Central NetCenter pelo
> nome, utilize o endereço IP configurado abaixo.

A Central NetCenter uma vez configurada, disponibiliza uma interface Web para a sua operação e/ou configuração
adicional, porém a configuração inicial deve ser feita através de uma 
[interface de linha de comandos](#interface-de-linha-de-comandos). Para acessar esta interface, utilize
uma das duas formas descritas abaixo:

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
#### Reiniciar o equipamento
```
atHome> reboot
```
>Algumas alterações nas interfaces de rede só surtem efeito após a reinicialização da Central NetCenter.

## Interface Web

Após a configuração inicial da Central NetCenter é possível acessá-la via interface Web através do
endereço ```http://athome.local``` ou ```http:*endereco_ip_configurado*```. A primeira tela disponibilizada
é a tela de login.
```
login: admin@home.com
senha: 1234
```
