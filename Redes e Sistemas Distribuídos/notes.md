<h1>Redes Distribuídas</h1>
<h2>Resumo</h2>
<p>Um rede distribuída é todo e qualquer conjunto de dispositivos e infraestrura pelo qual os dados trafegam, por exemplo uma rede estruturada de uma empresa, ou uma rede de transmissão da operadora de internet e telefonia</p>

<h2>O que são gargalos de rede?</h2>
<p>São fenomenos que limitam a capacidade ou performance de uma rede. Neste caso quando ocorre uma sobrecarga na rede, seja em conexões oiu em tráfego, temos um gargalo onde a rede não suporta o volume excedente e ocorre o efeito de funil.</p>
<h2>Modelo OSI</h2>
<p>É um modelo teórico, de referência, para a construção de uma rede. O modelo em questão foi proposto pela ISO como um passo inicial para a padronização dos protocolos e estruturas empregadas nas redes de computadores. Este caso não se trata de uma <i>arquitetura de rede</i> posto que o modelo OSI apenas propõe um <i>modelo de referência</i> a ser empregado em cada nível.</p>
<h3>Estrutura do Modelo OSI</h3>
<p>O modelo OSI é composto de 7 camadas conforme a tabela abaixo:<br/>
    <table style="border: 0.5px solid; ">
        <tr style="color: purple; font-weight:bold; text-align: center; font-size: 18px">
            <td>Nível</td>
            <td>Camada</td>
            <td>Descrição</td>
        </tr>
        <tr>
            <td>7</td>
            <td>Aplicação</td>
            <td>A camada de aplicação é aquela que contém os os protocolos que são usados pelas aplicações e usuários, como o HTTP/HTTPS, FTP, SSH, etc.</td>
        </tr>
        <tr>
            <td>6</td>
            <td>Apresentação</td>
            <td>É uma camada que serve para a execução de funçõs, compressão, criptografia e codificação dos dados. Diferente das demais camadas, a camada de apresentação se preocupa com a sintaxe dos daos, e não somente com os bits.</td>
        </tr>
        <tr>
            <td>5</td>
            <td>Sessão</td>
            <td>Esta camada permite que usuários de máquinas distintas possam estabelecer conexões entre sí, além de permitir a abertura de conxões remotas, transporte de dados, logins remotos, VPN's.</td>
        </tr>
        <tr>
            <td>4</td>
            <td>Transporte</td>
            <td>Está camada serve à camada de sessão, nela há a fragmentação dos dados de sessão para encaminhamento à rede, certificando-se que cheguem corretamente ao destino.</td>
        </tr>
        <tr>
            <td>3</td>
            <td>Rede</td>
            <td>Já a camada de rede é aquela onde esta o controle da sub-rede, ou seja, o conjunto de portas e interfaces que contém o endereçamento dos pacotes. É ela quem se preocupa como ocorre o roteamento dos pacotes entre uma origem e destino, nela também encontramos as tabelas estáticas ou dinâmicas de roteamento, desse modo também prevenindo congestionamentos no tráfego de dados.</td>
        </tr>
        <tr>
            <td>2</td>
            <td>Enlace</td>
            <td>Esta camada é a responsável por organizar e gerenciar a camada física, ou seja, ela quem comanda e gerencia a comunicação da camada física livre de erros, gerenciando e controlando o fluxo de bits.</td>
        </tr>
        <tr>
            <td>1</td>
            <td>Física</td>
            <td>Esta é a camada mais básica da rede, pela qual os bits brutos são processados e transmitidos por um canal (cabo, fibra ótica, par metálico, etc) nesta camada também está contido os controles de tempo de transmissão e transmissões simultâneas e sincronicidade.</td>
        </tr>
    </table>
</p>
<h2>Modelo TCP/Ip</h2>
<p>O modelo TCP/Ip, diferente do modelo OSI, é uma arquitetura de rede, inclusive a mais comum e padrão do mercado atual. O TCP/Ip se distingue do OSI em alguns pontos chave como a unificação das camadas de aplicação, sessão e apresentação, assim como das camadas fisicas e enlace, ou seja, este modelo tem apenas 4 camadas ao invés das 7 do modelo anteriormente proposto. Este modelo se baseia na comunicação com endereçamento por IP's, ou seja, um endereço numérico, único na rede, que define o dispositivo. A estrutura de Ip constitui-se de Ip's públicos e privados, ou seja, Ip's abertos à rede e outros apenas de uma rede interna (ou sub-rede) sendo que neste caso um pacote chega endereçado à um Ip publico e a subrede o endereça para o Ip privado alvo, sendo neste caso ela quem direciona as requisições e controla a troca de informações da subrede.</p>
<h3>Características do TCP/Ip</h3>
<p>O modelo TCP/Ip permite, entre diversas outras coisas, a independência de marcas e fabricantes, ou seja, torna todos os dispositivos compatíveis entre sí. Permite também que dois computadores que utilizem de uma conexão TCP/Ip se conectem e se comuniquem sem a necessidade de dispositivos intermediários. Além disso ela também conta com a oferta de descição de padrões para protocolos do nível de aplicação como o FTP, SMTP, Login remoto, SSH, etc.</p>
<table style="border: 1px solid">
    <tr style="color: purple; font-weight:bold; text-align: center; font-size: 18px">
        <td>Nível</td>
        <td>Camada</td>
        <td>Descrição</td>
    </tr>
    <tr>
        <td>4</td>
        <td>Aplicação</td>
        <td>A camada de aplicação reúne os protocolos os quais a rede trabalha assim como trata da sintaxe e semântica das mensagens e pacotes assim como trata dos detalhes de cada tipoo aplicação sendo implementada através de processos do próprio sistema operacional.</td>
    </tr>
    <tr>
        <td>3</td>
        <td>Transporte</td>
        <td>É a camada responsável pela comunicação end-to-end entre as aplicações utilizando os protocolos TCP e UDP para padronizar os pacotes trafegados.</td>
    </tr>
    <tr>
        <td>2</td>
        <td>Internet</td>
        <td>É a camada que reúne os endereços e roteamento dos pacotes entre os dispositivos da rede, ela quem também define o formato e o protocolo utilizado para o roteamento, o IP (Internet Protocol).</td>
    </tr>
    <tr>
        <td>1</td>
        <td>Interface de Rede</td>
        <td>Está é a camada de mais baixo nível nesta arquitetura, ela é quem é responsável pela tradução dos bits para sinais de transmissão, especificação dos meios de transmissão e do endereçamento e chaveamento dos pacotes.</td>
    </tr>
</table>
<h2>Principais Protocolos do TCP/Ip</h2>
<h3>TELNET (Telephone Network)</h3>
<p>É um protocolo que utiliza menor fluxo de dados, destinado ao serviço de terminal virtual (terminal linux ou prompt de comando / power-shell), ele também permite a conexão remota utilizando-se deste terminal.</p>
<h3>FTP (File Transfer Protocol)</h3>
<p>É um protocolo destinado ao transporte de arquivos via rede, utilizado geralmente para implementações de file-servers ou pastas compartilhadas na internet.</p>
<h3>SMTP (Simple Mail Transfer Protocol)</h3>
<p>Este é um protocolo que padroniza o gerenciamento e distribuição de e-mails na rede. Este protocolo possui, entre suas características, um conjunto de atributos de chaves e identificadores, para garantir a origem e destino das mensagens trafegadas.</p>
<h3>SMNP (Simple Network Management Protocol)</h3>
<p>É um protocolo destinado ao gerenciamento e administração da rede, ele permite a coleta e manipulação de informações geradas pela rede e também permite que possam ser observados comportamentos inesperados ou anomalos na rede.</p>
<h3>DNS (Domain Name System)</h3>
<p>É o protocolo utilizado para definir e mapear nomes em endereços de rede, ele quem permite utilizarmos palvras para navegar na internet ao invés de Ip's.</p>
<h3>HTTP (Hypertext Transfer Protocol)</h3>
<p>Trata do WWW, ou seja, o protocolo que permite a distribuição de sites e aplicações web mundialmente a partir de endereços DNS.</p>

<h2>TCP - Transmision Control Protocol</h2>
<p>Trata-se de um protocolo geral da arquitetura o qual carrega consigo um conjunto de definições para a mesma, entre elas temos a orientação à conexão, o fluxo confiável de dados, a segmentação do fluxo de dados. O TCP também permite a escolha de caminhos confiáveis, o estabelcimento de conexões end-to-end e a confirmação do recebimento de pacotes. Aléme disso o protocolo TCP possui a característica de possibilitar conexões elásticas com a confirmação do recebimento e retransmissão de pacotes em caso de falhas prevenindo a degradação do serviço.</p>
<h2>UDP - User Datagram Protocol</h2>
<p>O protocolo UDP, por sua vez, possui menos complexidade em sua aplicação, não sendo orientado à conexão e não possuindo tantos controles como o TCP, sendo considerado uma versão simplificada deste primeiro. O UDP apenas trafega os pacotes entre os dispositivos, não garantindo a entrega dos mesmos à aplicação bem como não oferece uma camada confiável quanto à transmissão e degradação do serviço. Sua principal utilização é com streamings, onde o fluxo contínuo de dados não requer tantos controles.</p>
<h2>Protocolos de Inter-Rede (Internet)</h2>
<h3>IP (Internet Protocol)</h3>
<p>A Internet utiliza, por padrão, o protocolo IP (Internet Protocol) onde o mesmo provê o endereçamento dos dispositivos para facilitar o roteamento dos pacotes dado que havendo um endereço real (IP) fica mais fácil e rastreável o tráfego de dados. Em conjunto a isso temos um serviço de datagrama não confiável pois, tal qual o UDP, este protocolo não se preocupa com o fluxo de dados, apenas com o roteamento e endereçamento dos datagramas entre dispositivos, o IP é quem roteia, envia e recebe datagramas IP.</p>
<h3>ICMP (Internet Control Message Protocol)</h3>
<p>É um protocolo que permite a troca de mensagens de erro no processamento de datagramas IP, ou seja, ele é destinado à troca de pacotes simples de erro na rede. Nele estão contidos o <i>Buffer Full, Hops, Ping e Traceroute</i>.</p>
<ul>
    <li>Buffer Full - Trata-se de um erro onde a rede encontra incapaz de atender novos pacotes devido sobrecarga ou congestionamento.</li>
    <li>Hops - É a contagem de saltos necessários para um pacote chegar ao seu destino, ou seja, por quantos nodos de rede o pacote transitou até ser recebido.</li>
    <li>Ping - É um tipo de pacote destinado à checar se um destino está acessível, neste caso ele pode responder tanto como inacessível como com time-out.</li>
    <li>Traceroute - permite o mapeamento de saltos necessários para um pacote atingir seu destino.</li>
</ul>
<h3>Protocolos Inferiores</h3>
<h4>IGMP (Internet Group Management Protocol)</h4>
<p>É um protocolo que controla o grupo de endereços de rede (IP's ou DNS's) onde o mesmo permite a visibilidade das tabelas e endereços.</p>
<h4>BGP, OSPF e RIP</h4>
<p>São protocolos para controle de roteamento, eles são responsáveis por transitar as informações de roteamento e redirecionamento de pacotes.</p>
<h4>ARP (Address Resolution Protocol)</h4>
<p>É um protocolo de uso específico, ele permite a comunicação direta entre dispositivos em rede quando apenas o IP é conhecido pelo destinatário dos pacotes.</p>
<h2>Camada de Interface de Rede: protocolos</h2>
<p>A camada de interface de rede também possui alguns protocolos específicos destinados ao tráfego e codificação dos bits para sinais de transmissão, estes protocolos definem pontos como endereçamentos, barramentos, enlaces e sub-redes. São muito empregados tanto para controle de tráfego e perfomance quanto para estruturação de sub-redes, no cascateamento de endpoints e firewalls.</p>