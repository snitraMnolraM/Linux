# Linux -  Introdução ao Sistema Operacional

### Capitulo 1 - Introdução ao Linux e Configuração Inicial

##### Instalação e configuração

Primeiro faça download do **VMware Workstation Player** é do ISO do **Ubuntu 20.04 LTS**.

|           SOFTWARE           |                 LINKS                    |
| :----------------------------: | :---------------------------------------: |
| VMWare Workstation Player 16 | https://www.vmware.com/go/getplayer-win  |
| Ubuntu 20.04 LTS             | https://ubuntu.com/download/desktop/thank-you?version=20.04.2.0&architecture=amd64 |

Instale o VMware Workstation Player. Ele é um utilitário ideal para executar uma única máquina virtual em um PC Windows ou Linux. Ao termino da instalação e emule o Ubuntu. 

​                                                                            `*Escolher no minímo 40GB de espaço para a maquina virtual`



<br />
<br />
<br />
<br />

#### Outra Forma de Baixar o Ubuntu 

 `caso o Link acima não Funcione`

Entre no endereço: [ubuntu.com]()

Clique na aba "Downloads"

Clique no link "**ubuntu desktop**"

Clique em "**Download**" da versão mais recente



<br />
<br />
<br />
<br />

### Capitulo 2 - Conhecendo o Terminal Linux e seus Atalhos

##### Conhecendo o terminal e primeiros comandos
<br />

Atalho para abrir o Terminal >> **CTRL +ALT + T**
<br />

|                  FUNÇÃO                  |         COMANDOS DENTRO DO TERMINAL                 |
| :--------------------------------------: | :--------------------------------------: |
|    Para voltar para diretório pessoal    |                   cd ~                   |
| Para informar o caminho do local onde estamos logado |                   pwd                    |
| Para listar os arquivos e pastas desse loca |                    ls                    |
|   Para listar os arquivos de uma pasta   |            ls (nome da pasta)            |
| Para listar pastas e arquivos com detalhes |                  ls -l                   |
| Para listar todos as pastas e arquivos da pasta pessoal |                   ls ~                   |
|    Para abrir o manual de um programa    |                  man ls                  |
|           Para sair do manual            |            h (ajuda) q (sair)            |
| Para abrir arquivo de ajuda em português |                ls -- help                |
|         Para entrar em uma pasta         |            cd (nome da pasta)            |
|      Para voltar uma pasta/caminho       |                  cd ..                   |
| Para sair do diretório pessoal para o diretório raiz |                   cd /                   |
|           Para criar uma pasta           |          mkdir (nome da pasta)           |
|          Para remover uma pasta          |          rmdir (nome da pasta)           |
|          Para remover arquivos           |           rm (nome do arquivo)           |
|    Para exibir histórico do terminal     |                 history                  |
|   Para executar o ultimo comando usado   |                    !!                    |
|  Para mover ou renomear um arquivo = mv  |                    mv                    |
|             Renomear a pasta             |    mv (nome pasta) (nome nova pasta)     |
|              Mover a pastar              |            mv (nome pasta) ~             |
|          Criar um arquivo vazio          |          touch (nome pasta).txt          |
|           Renomear um arquivo            |  mv (nome arquivo).txt (novo nome).txt   |
|              Copiar arquivo              | cp (nome arquivo).txt /home/anderson (diretório) |
|        Para completar uma palavra        |                tecla TAB                 |
|      Para limpar a tela do terminal      |                  clear                   |

`*Para rodar comandos como administrator (user "root") use sudo. Como no exemplo abaixo: `

```bash
sudo apt install xcowsay
```

 <br />
<br />



|                 FUNÇÕES                  | ATALHOS DO TERMINAL |
| :--------------------------------------: | :-----------------: |
| Cancela o comando atual em funcionamento |      CTRL + C       |
| Pausa o comando atual, em primeiro plano ou segundo plano |      CTRL + Z       |
|      Fazer o logout da sessão atual      |      CTRL + D       |
|     Apaga uma palavra na linha atual     |      CTRL + W       |
|          Apaga a linha inteira           |      CTRL + U       |
|         Busca um comando recente         |      CTRL + R       |
|             Sai do terminal              |        exit         |

<br />
<br />

<br />
<br />

### Capitulo 3 - Comandos para Manipulação de Arquivos, Textos e Redirecionamento

##### Lidando com arquivos .txt
<br />
<br />
Para abrir esse programa basta digitar no terminal = nano (nome do arquivo.txt)



|     EDITOR DE TEXTO DO LINUX - NANO      | COMANDO DENTRO DO NANO |
| :--------------------------------------: | :--------------------: |
|         Arquivo de Ajuda do nano         |        CTRL + G        |
|          Fechar o programa nano          |        CTRL + X        |
| Gravar no disco o arquivo (salvar arquivo) |        CTRL + O        |
|            Justificar o texto            |        CTRL + J        |
|            Desfazer uma ação             |        ALT + U         |
|             Refazer uma ação             |        ALT + E         |
|             Marcando o texto             |         ALT+ A         |
|         Copiar texto selecionado         |        ALT + 6         |
|              Colar um texto              |        CTRL +U         |
| Fazer a verificação da ortografia do texto |        CTRL + T        |
|    Substituir alguma palavra do texto    |        CTRL + \        |



<br />
<br />

|    PARA VISUALIZAR UM ARQUIVO DE TXT     |         COMANDOS DENTRO DO TERMINAL          |
| :--------------------------------------: | :------------------------: |
| Para visualizar um arquivo de txt sem abrir | cat (nome do arquivo.txt)  |
| Para visualizar o arquivo de txt, porém com as linhas invertidas |  tac (nome do arquivo.txt  |
| Para visualizar apenas as 10 primeiras linhas de um arquivo txt | head (nome do arquivo.txt) |
| Para visualizar apenas as 10 ultimas linhas de um arquivo txt | tail (nome do arquivo.txt) |

<br />
<br />

| PROPRIEDADES DO ARQUIVO .TXT E COMANDOS DE DATAS |                 COMANDOS DENTRO DO TERMINAL                 |
| :--------------------------------------: | :--------------------------------------: |
| Comando para adicionar uma informação dentro de um novo arquivo | tail (nome do arquivo.txt) > (nome do arquivo.txt) |
|  Cria uma informação dentro do arquivo   |                   (>)                    |
| Adicionar uma informação dentro de um arquivo já existente |      date >> (nome do arquivo.txt)       |
| Adiciona uma informação dentro do arquivo |                   (>>)                   |
| Para mostrar calendário do mês corrente  |                   cal                    |
|         Para mostrar data atual          |                   date                   |
|  Para busca uma palavra dentro do texto  |                   grep                   |
| Para procurar a palavra **palavras** nas 10 ultimas linha do arquivo.txt | tail (nome do arquivo.txt) \| grep palavras |



<br />
<br />

|           PAGINAÇÃO DE TEXTOS            |                 COMANDOS DENTRO DO TERMINAL                 |
| :--------------------------------------: | :--------------------------------------: |
| Para facilitar a leitura de um arquivo muito grande | more ou less ( cat (nome do arquivo.txt) \| more (Para parar de exibir bastar apertar CTRL + Z |
| Envia a saída de um comando para entrada de outro comando permitindo a execução de dois comandos |                    \|                    |
| Permite usar dois comandos e separar suas saídas no terminal |                    &                     |
| Usado para que dois comandos só sejam executados se o primeiro for executado com sucesso |                    &&                    |
| Usado para informar o que faz cada comando. ( whatis ls) (whatis find) |                  whatis                  |

<br />
<br />
<br />
<br />

### Capitulo 4 - Diretórios do Linux e Comandos de Sistema

#### Apresentação dos comandos de diretórios do linux
<br />
<br />
Diretórios importantes

|                  FUNÇÃO                  | DIRETÓRIO |
| :--------------------------------------: | :-------: |
|     Binários principais dos usuários     |   /bin/   |
|       Arquivos do sistema de Boot        |  /boot/   |
|         Arquivos de dispositivos         |   /dev/   |
|   Arquivos de configurações do sistema   |   /etc/   |
| Diretório dos usuários comuns do sistema |  /home/   |
| Bibliotecas essenciais do sistema e dos módulos do kernel |   /lib/   |
|   Diretório de montagem e dispositivos   |  /media/  |
| Diretório de montagem de dispostivos (Alternativo do /media/) |   /mnt/   |
| Instalação de programas não oficiais da distribuição por conta do usuário |   /opt/   |
| Armazena arquivos executáveis que representam comandos administrativos |  /sbin/   |
| Diretório para dados de serviços fornecidos pelo sistema |   /srv/   |
|   Diretório para arquivos temporários    |   /tmp/   |
| Segunda hierarquia do sistema, onde ficam os usuários comuns do sistema e programas. |   /usr/   |
| Diretório com arquivos variaveis gerados pleos programas do sistema |   /var/   |
|        Diretório do usuário root         |  /root/   |
| Diretório virtual controlado pelo Kernel |  /proc/   |

<br />
<br />



#### Praticando no terminal os comandos de diretórios e sistema
<br />
<br />


|                  FUNÇÃO                  | COMANDOS DENTRO DO TERMINAL |
| :--------------------------------------: | :-----------------: |
|     Ver informações do processamento     |  cat /proc/cpuinfo  |
|      Ver informações sobre memoria       |  cat /proc/meminfo  |
| Ver informações sobre placas conectadas no computador |        lspci        |
|   Ver informações de dispositivos usb    |        lsusb        |
| Ver a arquitetura do sistema que você está usando |        arch         |
|           Ver o nome do Kernel           |        uname        |
|          Ver a versão do Kernel          |      uname -r       |
|       Ver a arquitetura do Kernel        |      uname -m       |
| Mostra saída de memoria física e memória swape |        free         |
| Ver todo o diretório pessoal e quando ele usa de espaço de hd |       du -h ~       |
|     Ver todos os usuários do sistema     |   cat /etc/passwd   |
|           Reiniciar o sistema            |       reboot        |
|            Desligar o sistema            |   shutdown -h now   |
|           Reiniciar o sistema            |     shutdown -r     |
|   Ver todas as informações sobre o CPU   |        lscpu        |
| Ver uma lista de todos os hardwares que o sistema encontrar |        lshw         |
|      Mostrar o caminho de hardwares      |     lshw -short     |

<br />
<br />
<br />
<br />



### Capitulo 5 - Fundamentos de Rede e Comandos de Rede

#### O que são Redes, Protocolos e Interfaces de Rede

<br />

- **O que é Rede ?**

  Rede é um conjunto de equipamentos interligados de maneira a trocarem informações e compartilham recursos.

  ​

  - Rede Wan

    Wide Area Network ou World Area Network é uma rede geograficamente distribuída

    ​

  - Rede Man

    Metropolitan Area Network é uma rede metropolitana que interligam várias redes locais

    ​

  - Rede Lan

    Local Area Network é uma rede local de uma forma geral em um único prédio ou campus

<br />
<br />

- **Protocolos**	

  Protocolo é a "linguagem" usada pelos dispositivos de uma rede de modo que eles consigam se 	entender. Existem vários protocolos


  ​

  - Protocolo IP

    Protocolo de Internet - Endereço IP - Número que identificam seu computador em uma rede

    ​

  - Protocolo ICMP (Internet Control Message Protocol)

    Tem por objetivo prover mensagens de controle na comunicação entre nós

    ​

  - DNS (Domain Name Server)

    Esse protocolo de aplicação tem por função identificar endereços IPs e manter uma tabela com os endereços dos caminhos de algumas redes

<br />
<br />



- **Interface de Rede**

  Interface de rede é um software e/ou hardware que faz a comunicação em uma rede de computadores.
  As Interfaces de rede no linux estão localizadas no diretório /dev e a maioria é criada dinamicamente pelos softwares quando são requisitadas.

  ​

  - Interface de Rede (Loopback)

    A interface loopback é um tipo especial de interface que permite fazer conexões com você mesmo, com ela, você pode testar vários programas de rede sem interferir em sua rede. O endereço padrão para o loopback é IP 127.0.0.1
