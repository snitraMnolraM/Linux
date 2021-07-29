# Linux -  Introdução ao Sistema Operacional

### Capitulo 1 - Introdução ao Linux e Configuração Inicial

##### Instalação e configuração

Primeiro faça download do **VMware Workstation Player** é do ISO do **Ubuntu 20.04 LTS**.

| SOFTWARE                     | LINKS                                    |
| ---------------------------- | :--------------------------------------- |
| VMWare Workstation Player 16 | https://www.vmware.com/go/getplayer-win  |
| Ubuntu 20.04 LTS             | https://ubuntu.com/download/desktop/thank-you?version=20.04.2.0&architecture=amd64 |

Instalamos o VMware Workstation Player. Ele é um utilitário ideal para executar uma única máquina virtual em um PC Windows ou Linux. Ao termino da instalação e emule o Ubuntu. 

​                                                                            `*Escolher no minímo 40GB de espaço para a maquina virtual`





Outra Forma de Baixar o Ubuntu, caso o Link acima não Funcione

entrar no endereço: ubuntu.com

clicar na aba "downloads"

clicar no link "ubuntu desktop"

clicar em "download" da versão mais recente





### Capitulo 2 - Conhecendo o Terminal Linux e seus Atalhos

##### Conhecendo o terminal e primeiros comandos



|                  FUNÇÃO                  |                 COMANDOS                 |
| :--------------------------------------: | :--------------------------------------: |
|           Acessando o Terminal           |              CTRL +ALT + T               |
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

 



|                 FUNÇÕES                  | Atalhos do Terminal |
| :--------------------------------------: | :-----------------: |
| Cancela o comando atual em funcionamento |      CTRL + C       |
| Pausa o comando atual, em primeiro plano ou segundo plano |      CTRL + Z       |
|      Fazer o logout da sessão atual      |      CTRL + D       |
|     Apaga uma palavra na linha atual     |      CTRL + W       |
|          Apaga a linha inteira           |      CTRL + U       |
|         Busca um comando recente         |      CTRL + R       |
|             Sai do terminal              |        exit         |



### Capitulo 3 - Comandos para Manipulação de Arquivos, Textos e Redirecionamento

##### Lidando com arquivos .txt

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





|    PARA VISUALIZAR UM AQRUIVO DE TXT     |          COMANDOS          |
| :--------------------------------------: | :------------------------: |
| Para visualizar um arquivo de txt sem abrir | cat (nome do arquivo.txt)  |
| Para visualizar o arquivo de txt, porém com as linhas invertidas |  tac (nome do arquivo.txt  |
| Para visualizar apenas as 10 primeiras linhas de um arquivo txt | head (nome do arquivo.txt) |
| Para visualizar apenas as 10 ultimas linhas de um arquivo txt | tail (nome do arquivo.txt) |



| PROPRIEDADES DO ARQUIVO .TXT E COMANDOS DE DATAS |                 COMANDOS                 |
| :--------------------------------------: | :--------------------------------------: |
| Comando para adicionar uma informação dentro de um novo arquivo | tail (nome do arquivo.txt) > (nome do arquivo.txt) |
|  Cria uma informação dentro do arquivo   |                   (>)                    |
| Adicionar uma informação dentro de um arquivo já existente |      date >> (nome do arquivo.txt)       |
| Adiciona uma informação dentro do arquivo |                   (>>)                   |
| Para mostrar calendário do mês corrente  |                   cal                    |
|         Para mostrar data atual          |                   date                   |
|  Para busca uma palavra dentro do texto  |                   grep                   |
| Para procurar a palavra **palavras** nas 10 ultimas linha do arquivo.txt | tail (nome do arquivo.txt) \| grep palavras |





|           PAGINAÇÃO DE TEXTOS            |                 COMANDOS                 |
| :--------------------------------------: | :--------------------------------------: |
| Para facilitar a leitura de um arquivo muito grande | more ou less ( cat (nome do arquivo.txt) \| more (Para parar de exibir bastar apertar CTRL + Z |
| Envia a saída de um comando para entrada de outro comando permitindo a execução de dois comandos |                    \|                    |
| Permite usar dois comandos e separar suas saídas no terminal |                    &                     |
| Usado para que dois comandos só sejam executados se o primeiro for executado com sucesso |                    &&                    |
| Usado para informar o que faz cada comando. ( whatis ls) (whatis find) |                  whatis                  |

