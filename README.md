 # Projeto_final
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
**user.name:**configuração de e-mail ao acesso do git

## Clonando repositório
`git clone https://github.com/fulano/rails-ini.git` 
**git clone:** copiar um repiar repositório de um git existente


# instalação de Vagrant  (virtual Box)
Nesta sessão será  os comandos para instalação e configuração da máquina virtual para  preparação de ambientação para execução.

	> To start syncing your workspace, just sign in with Google in the menu.

- Conceito de vagrant 
	> **Vagrant** são as máquinas virtuais que de fato irão rodar o SO. Pense na boxe como um HD com um sistema instalado e configurado pronto para ser utilizado. A **box** deve ser definida pela entrada config. vm.

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

> **_Vagrantfile_:**  O arquivo _Vagrantfile_ é o arquivo de configuração do _Vagrant_ para o seu projeto. É nele que definimos tudo da sua maquina virtual
```mermaid
`Vagrant.configure("2") do |config| 
config.vm.box = "GuiDev/Ubuntu-Rails5x"
config.vm.box_version = "1.0.0"
config.vm.network :forwarded_port, guest: 3000, host: 3000 
config.vm.network :forwarded_port, guest: 5432, host: 5432
config.vm.provider "virtualbox" do |vb|
vb.gui = true
vb.memory = "1024"
   end 
 end
```

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

## Verificar versões de inetalações
`vagrant ssh`

SmartyPants converts ASCII punctuation characters into "smart" typographic punctuation HTML entities. For example:

|                |ASCII                          |HTML                         |
|----------------|-------------------------------|-----------------------------|
|Single backticks|`'Isn't this fun?'`            |'Isn't this fun?'            |
|Quotes          |`"Isn't this fun?"`            |"Isn't this fun?"            |
|Dashes          |`-- is en-dash, --- is em-dash`|-- is en-dash, --- is em-dash|


## KaTeX

You can render LaTeX mathematical expressions using [KaTeX](https://khan.github.io/KaTeX/):

The *Gamma function* satisfying $\Gamma(n) = (n-1)!\quad\forall n\in\mathbb N$ is via the Euler integral

$$
\Gamma(z) = \int_0^\infty t^{z-1}e^{-t}dt\,.
$$

> You can find more information about **LaTeX** mathematical expressions [here](http://meta.math.stackexchange.com/questions/5020/mathjax-basic-tutorial-and-quick-reference).


## UML diagrams

You can render UML diagrams using [Mermaid](https://mermaidjs.github.io/). For example, this will produce a sequence diagram:

```mermaid
`Vagrant.configure("2") do |config| 
config.vm.box = "GuiDev/Ubuntu-Rails5x"
config.vm.box_version = "1.0.0"
config.vm.network :forwarded_port, guest: 3000, host: 3000 
config.vm.network :forwarded_port, guest: 5432, host: 5432
config.vm.provider "virtualbox" do |vb|
vb.gui = true
vb.memory = "1024"
   end 
 end
```
