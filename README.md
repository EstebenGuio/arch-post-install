# Post arch linux script (Español):

## Funcionalidades:

### Actualización keys

    $   sudo pacman -Sy archlinux-keyring
    $   sudo pacman -Syu

    
### configuraciones git 

    $   cd ~
    $   ssh-keygen -o -t rsa -C "your-email@gmail.com"
    -   Go to  [https://github.com/settings/keys](https://github.com/settings/keys)
    $   cat id_rsa.pub
    -   Copy the text and create the new key in github
    $   sudo pacman -S git
    $   git config --global user.name "You name"
    $   git config --global user.email "your-email@gmail.com"

### Quitar vim e instalar neovim
    $   sudo pacman -R vim && sudo pacman -S neovim

### Instalar python (para usar pycritty)

    $   sudo pacman -S python-pip
    $   pip install --install-option="--themes=all" pycritty
    $   export PATH=$HOME/.local/bin:$PATH

Seguir las instrucciones en el link abajo
[https://github.com/antoniosarosi/pycritty](https://github.com/antoniosarosi/pycritty)

### Instalar visual studio code

    $   sudo pacman -S code

### Enable natural scrolling
    $   nvim /etc/X11/xorg.conf.d/XX-touchpad.conf
        Add the option:
        Option "NaturalScrolling" "true"

### Download fonts
    $   cd /usr/share/fonts
    $   sudo su
    $   rm -rf *
    $   wget https://github.com/ryanoasis/nerd-fonts/releases/download/v2.2.2/3270.zip && wget https://github.com/ryanoasis/nerd-fonts/releases/download/v2.2.2/UbuntuMono.zip && wget https://github.com/ryanoasis/nerd-fonts/releases/download/v2.2.2/Mononoki.zip && wget https://github.com/ryanoasis/nerd-fonts/releases/download/v2.2.2/JetBrainsMono.zip
    $   unzip *.zip

### Download qtile configuration:

    Leer el repo antes de clonar
    $   cd ~/.config
    $   rm -rf qtile
    $   git clone https://github.com/estebenguio/qtile
    

### Instalar nodejs
    $   sudo pacman -S nodejs npm # For latest version
    $   sudo pacman -S nodejs-lts-gallium npm # For 16 version
    $   sudo pacman -S 	nodejs-lts-hydrogen npm # for 18 version

### Instalar jdk
    $   sudo pacman -S jdk11-openjdk

### Instalar JetBrains
    $   wget https://download.jetbrains.com/toolbox/jetbrains-toolbox-1.27.2.13801.tar.gz
    $   tar -zxvf jetbrains-toolbox*.tar.gz
    $   cd jetbrains*
    $   .
    /jetbrains*
    -   Manage your IDES from here
    
### Instalar brave
    $ sudo pacman -S brave

### Docker
### kubernetes
### 
    
