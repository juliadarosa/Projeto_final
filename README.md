# Comandos  utilizados em projeto!

Nesta documentação será reportada os comandos mais comuns e utilizados para para programação com a linguagem Raby rails, sendo dos passos iniciais para  instalação  de máquina virtual até as execuções de comandos e criação do banco de dados de aplicação.


# Acesso ao git e criação de repositório

Comando de acesso ao git e criação de repositório

## configurando usúario
`git config --global user.name “nome”` 

**git config:** configuração de git 

**user.name:** configuração de usúario

## Configuração de e-mail
`git config --global user.email “fulano……@...”` 

**git config:** configuração de git the tree.

**user.name:** configuração de e-mail ao acesso do git

## Clonando repositório
`git clone https://github.com/fulano/rails-ini.git`

**git clone:** copiar um repiar repositório de um git existente


# instalação de Vagrant  (virtual Box)
Nesta sessão será  os comandos para instalação e configuração da máquina virtual para  preparação de ambientação para execução.

## Instalação plugin de Vagrant
`Vagrant plugin install vagrant-vbguest`

**Vagrant plugin:** plugin de vagrant 

**install vagrant-vbguest  :** instalação de plugin virtual box


## Instalando VagrantFile
`vagrant init GuiDev/Ubuntu-Rails5x --box-version 1.0.0`

**vagrant init  :** criação de processos aprtir de script armazenado

**GuiDev/Ubuntu-Rails5x  :** script armazeando

**box-version 1.0.0  :** versão de máquina

## Configurando VagrantFile

> **Vagrantfile:**  O arquivo _Vagrantfile_ é o arquivo de configuração do _Vagrant_ para o seu projeto. É nele que definimos tudo da sua maquina virtual


	Vagrant.configure("2") do |config| 
	config.vm.box = "GuiDev/Ubuntu-Rails5x" 
	config.vm.box_version = "1.0.0" config.vm.network :forwarded_port, guest: 3000, host: 3000 
	config.vm.network :forwarded_port, guest: 5432, host: 5432 
	config.vm.provider "virtualbox" do |vb| 
	vb.gui = true vb.memory = "1024" 
		end 
	end

Como deve ser salvo arquivo .
Configurações da máquina virtual Box

# Comandos de status
 Comandos para serem realizados no Vangrant para definicção de Status de máquina Virtual.
 
## Iniciando Vagrant
`vagrant up`

**Vagrant:** Virtual Box

**UP:** iniciar Máquina virtual

## Suspender Vagrant
`vagrant suspend`

**Vagrant:** Virtual Box

**suspend:** comando de suspenção

## Parar Vagrant

`vagrant halt`
**Vagrant:** Virtual Box

**halt:** comando de parar Vagrant

# Acessando a máquina e verificação
comandos de  para acessar o ambiente de máquina virtual e verifação de  versionamento.
`vagrant ssh`

**Vagrant:** Virtual Box

**ssh:** autenticação para conectar a máquina virtual


# Verificar versões de inetalações
Verificação de versões de programas a serem utilizados para aplixações e desenvolvimento.

## Verificar versões de instalações

`Ruby -v`

**Ruby:** Progama  para estrurar e desenver sistemas web

**-v:** Versão 

`Rails -v`

**Rails:**  framework para o desenvolvimento de aplicações web

**-v:** Versão 

## instalar Rails
Comando para instalação de Rails

`gem install rails`

**gem:** gerenciador de dependencias de projeto

**install rails** Comando para instalação de rails

- Instalar versão especifica do Rails:
 
`gem install rails -v 5.2.8`

**gem:** gerenciador de dependencias de projeto

**install rails** Comando para instalação de rails

**install rails -v 5.2.8`** versão

# Acesso a pastas compartilhadas
Como navegar palas pastas compartilhadas no Vangrant
Comandos: 

- Sair da pasta
- 
`cd ..` 

- Listar arquivos da pasta

 `ls` 

- Acessar  arquivos da pasta
- 
`cd vagrant` 

# Instalar RVM para desenvolvimento em Ruby
> **RVM**  é uma ferramenta versátil que pode ser usada **_para gerenciar projetos e ambientes Ruby inteiros_**

Segue comando de instalação:
`rvm install 2.3` 

**rvm:**  ferramente para genreciar

**install 2.3** instalação e versão


# Programando em Ruby
Segue então alguns comandos de criação de aqruivos e alguns exemplos de como seria um cógigo em ruby puro

## Utilização de Ruby puro sem tratamentos
- Comando de criação de arquivos em ruby:

`ruby nome_arquivo.rb` 

- Desenvolvimento em Ruby:
>
	irb
	puts"“teste direto” “Feijao e bao demais”.reverse 
	exit

- criar pasta  em Ruby:
`rails new nome_pasta` 

Em resumo comandos básicos para serem utilizados em progrmação de Ruby sem tratativa

## Rodar pasta no servidor

`cd nome_pasta` 

**cd:** acessa a pasta que está sendo passada em comando

> Quando já esta em pasta para ser inicada em servidor roda o comendo :

`rails server -> rails s -b 0.0.0.0`

Assim acessa localhost em navegador e poderá ter acesso ao que já foi programado até o momento.





|                |ASCII                          |HTML                         |
|----------------|-------------------------------|-----------------------------|
|Single backticks|`'Isn't this fun?'`            |'Isn't this fun?'            |
|Quotes          |`"Isn't this fun?"`            |"Isn't this fun?"            |
|Dashes          |`-- is en-dash, --- is em-dash`|-- is en-dash, --- is em-dash|




> You can find more information about **LaTeX** mathematical expressions [here](http://meta.math.stackexchange.com/questions/5020/mathjax-basic-tutorial-and-quick-reference).


## UML diagrams

