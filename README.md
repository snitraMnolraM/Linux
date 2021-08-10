# Linux -  Introdução ao Sistema Operacional

### Capítulo 1 - Introdução ao Linux e Configuração Inicial

##### Instalação e configuração

Primeiro faça o download do **VMware Workstation Player** e do ISO do **Ubuntu 20.04 LTS**.

|           SOFTWARE           |                 LINKS                    |
| :----------------------------: | :---------------------------------------: |
| VMWare Workstation Player 16 | https://www.vmware.com/go/getplayer-win  |
| Ubuntu 20.04 LTS             | https://ubuntu.com/download/desktop/thank-you?version=20.04.2.0&architecture=amd64 |

Instale o VMware Workstation Player. Ele é um utilitário ideal para executar uma única máquina virtual em um PC Windows ou Linux. Ao terminar a instalação emule o Ubuntu com o programa. 

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

### Capítulo 2 - Conhecendo o Terminal Linux e seus Atalhos

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

`*Para rodar comandos como administrador (user "root") use sudo. Como no exemplo abaixo: `

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

### Capítulo 3 - Comandos para Manipulação de Arquivos, Textos e Redirecionamento

#### Lidando com arquivos .txt
<br />
<br />

Para abrir esse programa basta digitar no terminal >> **nano (nome do arquivo.txt)**
<br />

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

### Capítulo 4 - Diretórios do Linux e Comandos de Sistema

#### Apresentação dos comandos de diretórios do linux
<br />
<br />

**Diretórios importantes**
<br />

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



### Capítulo 5 - Fundamentos de Rede e Comandos de Rede

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
    
    
    
    
    #### Comando ifconfig

<br />

|          FUNÇÃO          |    COMANDOS NO TERMINAL    |
| :----------------------: | :------------------------: |
| Para saber IP da maquina |          ifconfig          |
| Para instalar o ifconfig | sudo apt install net-tools |

<br /><br />

#### Comandos Hostname e ping

<br />

|                  FUNÇÃO                  |        COMANDO DENTRO DO TERMINAL        |
| :--------------------------------------: | :--------------------------------------: |
|        Nome do computador na rede        |                 hostname                 |
|          Número de endereço IP           |               hostname -I                |
|       Número de endereço loopback        |               hostname -i                |
| Mostra informações completas do usuário  |                    w                     |
| Mostra informações curtas do usuário: Nome, data e horário de como estamos logado |                   who                    |
|     Mostra o nome do usuário logado      |                  whoami                  |
| Mostra informações completas sobre um site |     whois ( whois www.pudim.com.br )     |
|      Verifica se o host está ativo       | ping ( ping www.google.com.br ) (CTRL + Z para parar de pingar) |
|       Mostra informações sobre DNS       |        diq ( diq www.google.com )        |
|      Mostra somente o endereço DNS       |  dig +short (dig www.google.com +short)  |

 <br />
 <br />
 

#### Comandos Traceroute e finger

**Para traçar a rota da nossa rede local até um determinado host**

<br />


|                  FUNÇÃO                  |     COMANDO NO TERMINAL     |
| :--------------------------------------: | :-------------------------: |
|    Comando para instalar o traceroute    | sudo apt install traceroute |
| Traça a rota de um host até outro host ( traceroute www.google.com ) |         traceroute          |

<br />


#### Para mostra toda a informação do usuário que esta logado em nosso host

<br />


|                  FUNÇÃO                  |   COMANDO NO TERMINAL   |
| :--------------------------------------: | :---------------------: |
|          Para instalar o finger          | sudo apt install finger |
| Mostrar todos os usuários logados e informações, como nome, e tempo logado. |         finger          |

<br />
<br />
<br />
<br />

### Capítulo 6 - Fuçando no Linux com comandos diversos

#### Comandos history, alias e outras interações com arquivos .txt


<br />


|                  FUNÇÃO                  |    COMANDO NO TERMINAL     |
| :--------------------------------------: | :------------------------: |
| Menu Opções / Preferências / Criar Perfil / Mudar font e Tamanho | Aumentar letra do Terminal |
| Apagar histórico de comandos utilizados no Terminal |         history -c         |
| Dá um nome para outro comando (alias hh='history') |           alias            |
| Conta o número de linhas de um arquivo: nl (nome do arquivo.txt) |             nl             |
| Também conta o número de linhas, porém conta as linhas em branco: wc -l ( nome do arquivo.txt ) |           wc -l            |
| Conta o número de palavras dentro de um arquivo txt: wc -w (nome do arquivo.txt) |           wc -w            |
| Conta o número de bits do arquivo: wc -c (nome do arquivo) |           wc -c            |
| Conta o número de caracteres: wc -m (nome do arquivo) |           wc -m            |
| Mostra os arquivos e diretório ocultos (serão mostrados com um ponto antes: .local) |           ls -a            |
|   Mostra os diretórios com o / no fim    |           ls -F            |
| Comparar dois arquivos txt: cmp (nome do arquivo) (nome do arquivo) |            cmp             |
| Gera outra diferença entre arquivos txt: diff (nome do arquivo) (nome do arquivo) |            diff            |
| Organiza a saída do arquivo em ordem numérica |          sort -n           |
| Organiza a saída do arquivo em ordem alfabética |            sort            |
| Exibe o caminho do programa e seu manual |          whereis           |
|       Exibe o caminho de programa        |           which            |
|           Finaliza uma Sessão            |           logout           |

<br />


<br />


#### Comandos last reboot, route, time, cowsay e cmatrix

<br />


|                  FUNÇÃO                  |   COMANDO NO TERMINAL    |
| :--------------------------------------: | :----------------------: |
| Para mostrar todas as informações sobre a reinicialização do sistema |       last reboot        |
| Mostra todas as tabelas de roteamento e ip do Kernel |         route -n         |
| Mostra o tempo de um processo leva para ser processado<br /> (time traceroute www.google.com) |           time           |
| Mostra o tempo que o sistema está rodando |          uptime          |
| Para instalar o cowsay (Desenho Vaquinha) | sudo apt install cowsay  |
|     Mostra uma vaquinha com a frase      |   cowsay "Linux é Bom"   |
| Mostra uma vaquinha com a frase (com outra opção de rosto) |    cowsay -d "Linux"     |
| Mostra uma vaquinha com a frase (com outra opção de rosto) |    cowsay -g "Linux"     |
|  Mostra vários outros tipos de animais   |        cowsay -f         |
| Para instalar o cmatrix (Imita Efeito Filme Matrix) | sudo apt install cmatrix |
| Para instalar xcowsay (Desenho Vaquinha 3D) | sudo apt install xcowsay |

<br />

<br />



#### Comandos para desligar o sistema operacional

<br />


|                  FUNÇÃO                  | COMANDO NO TERMINAL |
| :--------------------------------------: | :-----------------: |
|      Desliga a máquina de imediato       |       init 0        |
|      Desliga a máquina de imediato       |      telinit 0      |
| Desliga a máquina, mas pede uma autenticação |        halt         |
| Imprimi uma sequência de números: (seq 1 10) |         seq         |

<br />

<br />

<br />

<br />


### Capítulo 7 - Controle de Usuários, Grupos e Permissões

#### Como Adicionar Usuários

<br />

|              FUNÇÃO              |      COMANDO NO TERMINAL       |
| :------------------------------: | :----------------------------: |
|    Para adicionar um usuário     |   adduser (nome do usuário)    |
| Comando usado como administrador | sudo adduser (nome do usuário) |

<br />

 

#### Como Trocar de Usuário e Alterar sua Senha

<br />

|             FUNÇÃO              |   COMANDO NO TERMINAL    |
| :-----------------------------: | :----------------------: |
|     Para trocar de usuário      |   su (nome do usuário)   |
| Para trocar para o usuário root |         sudo su          |
|  Para trocar senha do usuário   | passwd (nome do usuário) |

<br />

<br />

#### Como Exibir Informações de Login e Remover um Usuário

<br />

|                  FUNÇÃO                  |     COMANDO NO TERMINAL      |
| :--------------------------------------: | :--------------------------: |
| Para exibir informações de todos usuários do sistema |           lastlog            |
| Para exibir uma listagem de entrada e saída dos usuários do sistema |             last             |
| Para exibir o nome do usuário logado no sistema |           logname            |
| Para exibir os identificadores do usuário |              id              |
|      Para exibir todos os usuários       |       cat /etc/passwd        |
|         Para remover um usuário          |  userdel (nome do usuário)   |
| Para remover um usuário e a Pasta Pessoal do mesmo | userdel -r (nome do usuário) |




<br />

<br />

#### Como Criar um Grupo e Gerenciar os Usuários

**Grupos Permitem organizar os usuários e definir as permissões de acesso a arquivos e diretórios de forma mais fácil.**

<br />

|                  FUNÇÃO                  |           COMANDO NO TERMINAL            |
| :--------------------------------------: | :--------------------------------------: |
| Para visualizar todos os grupos do sistema |              cat /etc/group              |
| Para exibir todos os grupos de um usuário |                  groups                  |
|           Para criar um grupo            |      sudo addgroup (nome do grupo)       |
|   Para adicionar um usuário a um grupo   |  adduser (nome usuário) (nome do grupo)  |
|   Para adicionar um usuário a um grupo   | gpasswd -a (nome usuário) (nome do grupo) |
|   Para remover um usuário de um grupo    | gpasswd -d (nome usuário) (nome do grupo) |
|      Comando para remover um grupo       |                groupedel                 |

<br />

<br />

#### Como Gerenciar Permissões em Diretórios e o que é o modo octal



**Permissões em arquivos e diretórios servem para restringir acessos como: leitura, escrita e execução**

<br />

r = read (leitura)

w - write (escrita)

x - execution (execução)

<br />

<br />

#### Verificar Permissões em um diretório

<br />

|                  FUNÇÃO                  | COMANDO NO TERMINAL |
| :--------------------------------------: | :-----------------: |
| Mostra informações detalhadas sobre a pasta atual e suas permissões |       ls -lh        |
| Para mudar a permissão de um arquivo ou diretório |        chmod        |

<br />

d = (diretório) , - = (arquivo)

(sequencia de 9 dígitos) sendo que a cada 3 dígitos são separados por grupo, é o símbolo (-) significa que não tem acesso >> **rwxr-xr-x** 

1º grupo (dono/usuário) >> **rwx (permissões de r / w / x)**

2º grupo (grupo) >> **r-x (permissões de r / x ) (não permitido w)**

3° grupo (outros) >> **r-x (permissões de r / x) (não permitido w)**


<br />

<br />

#### Modo Octal

A máscara octal é composta por números sob a base 8 ou seja de 0 a 7 onde:

O primeiro dígito representa o dono do ficheiro/diretório (u)

O segundo dígito representa o grupo (g)

O terceiro dígito representa os outros (o)

As permissões são especificadas para cada grupo


<br />

|                  FUNÇÃO                  | COMANDO NO TERMINAL |
| :--------------------------------------: | :-----------------: |
|          Atribuição de r (read)          |          4          |
|         Atribuição de w (write)          |          2          |
|       Atribuição de x (execution)        |          1          |
| Atribuição para não ter nenhuma permissão |          0          |



<br />

<br />

#### Comando chmod

**Para colocar mais de uma situação ao arquivo/diretório, devemos somar os valores do grupo em que queremos alterar.**

Usando o comando >> **chmod 700 (nome do arquivo.txt)**  Essa atribuição significa que somente o grupo 1 (dono/usuário) tem permissão para r/w/x (read, write, execution)

Usando o comando >> **chmod 100 (nome do arquivo.txt)**  Essa atribuição significa que somente o grupo 1 (dono/usuário) tem permissão para executar

Usando o comando >> **chmod 755 (nome do arquivo.txt)**  Significa que o grupo 1 (dono/usuário) tem permissão r/w/x , que o grupo 2 (grupo) tem permissão r/-/x  e que o grupo 3 (outro) tem permissão r/-/x


<br />

<br /><br />

<br />



### Capitulo 8 - Compactação, Descompactação e Arquivamento

#### Comandos gzip, zip e bzip2 

<br />

**Compactadores são programas que diminuem o tamanho de um arquivo ou diretório**

<br />

**Extensões:**

As extensões identificam o tipo de um arquivo e o programa necessário para manipular o mesmo, dezenas de extensões identificam arquivos compactados, quando um arquivo é compactado, uma extensão é adicionada ao nome do arquivo.

<br /><br />

**Compactador Gzip**:

|             FUNÇÃO             |       COMANDO NO TERMINAL       |
| :----------------------------: | :-----------------------------: |
|         Para compactar         |   gzip (nome do arquivo.txt)    |
|       Para descompactar        | gunzip (nome do arquivo.txt.gz) |
| Para compactar com taxa máxima |  gzip -9 (nome do arquivo.txt)  |



<br /><br />

**Compactador Zip:**

|      FUNÇÃO      |           COMANDO NO TERMINAL            |
| :--------------: | :--------------------------------------: |
|  Para compactar  | zip (nome do arquivo.zip) (nome do arquivo.txt) |
| Para descompactar |       unzip (nome do arquivo.zip)        |

`*Pode colocar vários arquivos dentro de um único arquivo zipado`


<br /><br />

**Compactador Bzip2:**

|      FUNÇÃO       |        COMANDO NO TERMINAL         |
| :---------------: | :--------------------------------: |
|  Para compactar   |    bzip2 (nome do arquivo.txt)     |
| Para descompactar | bzip2 -d (nome do arquivo.txt.bz2) |

<br /><br />

**Comandos rar e tar**


|       FUNÇÃO        |           COMANDO NO TERMINAL            |
| :-----------------: | :--------------------------------------: |
| Para instalar o rar |           sudo apt install rar           |
|   Para compactar    | rar a (nome do arquivo.rar) (nome do arquivo.txt) |
|  Para descompactar  |       rar -x (nome do arquivo.rar)       |

 `*Esse comando necessita ser instalado na sua primeira utilização`

<br /><br />

**Arquivadores:**

Um arquivador junta vários arquivos em um só, mas pode ser usado em conjunto com um compactador para armazenar arquivos compactados;


|    FUNÇÃO     |           COMANDO NO TERMINAL            |
| :-----------: | :--------------------------------------: |
| Para arquivar | tar -cf (nome arquivo.tar) (nome arquivo.txt) (nome arquivo.txt) |

<br /><br />

**Esse arquivo pode ser compactado por outros compactadores.**

|               FUNÇÃO               |           COMANDO NO TERMINAL            |
| :--------------------------------: | :--------------------------------------: |
|   Para descompactar arquivo.tar    |    tar -xvf (nome do arquivo.tar.gz)     |
| Extrair o arquivo para outra pasta | tar -xvf (nome arquivo.tar.gz) -C ~/Pasta |


