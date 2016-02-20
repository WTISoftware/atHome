# NetCenter

A Central de Automação @home é um gateway que interliga todos os módulos instalados com a rede WiFi. Sua topologia sem fio permite comunicação rápida e eficaz entre os módulos, independente do seu local de instalação. A Central permite que todas as funcionalidades da linha @home sejam acessadas através de smartphones, tables e notebooks, assim como o agendamento de tarefas, a programação de cenários e o acesso remoto. 
Promove a interação com diversos tipos de sensores, proporciona total integração com equipamentos multimídias. Além de permitir o controle e dimerização personalizadas de lâmpadas ou leds.

1. [Instalação](#instalação)
2. [Configuração Inicial](#configuração)
   * [Através de um computador interligado](#através-de-um-computador-interligado)
   * [Através de um teclado USB e monitor HDMI](#através-de-um-teclado-usb-e-monitor-hdmi)
   * [Interface de linha de comandos](#interface-de-linha-de-comandos)

## Instalação

A central NetCenter pode ser instalada em qualquer lugar que seja possível a interligação com pelo menos
um módulo da tecnologia atHome. Ela é totalmente sem fio, e só precisa estar ligada à rede elétrica.

## Configuração

A Central NetCenter uma vez configurada, disponibiliza uma interface Web para a sua operação e/ou configuração
adicional, mas a configuração inicial deve ser feita através de uma interface de linha de comandos.

### Através de um computador interligado

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

### Através de um teclado USB e monitor HDMI
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
#### Interfaces de rede
A Central NetCenter possui duas interfaces de rede. Uma cabeada localizada na parte traseira do equipamento,
chamda de *lan* e outra wireless embutida chamada de *wlan*.

#### Visualizar interfaces de rede
```
atHome> show network status
```
#### Habilitar a interface cabeada
```
atHome> set lan mode enabled
```
#### Configurar a interface cabeada para DHCP
```
atHome> set lan mode dhcp
```
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
