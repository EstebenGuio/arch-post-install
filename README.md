# Post arch linux script (Español):

## Funcionalidades:

### Actualizar y usar mejores mirros: 

    $   sudo pacman -Syy
    $   sudo pacman -Scc

    
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
    $   pip install pycritty

    Seguir las instrucciones [aquí](https://github.com/antoniosarosi/pycritty)

### Instalar visual studio code

    $   sudo pacman -S code

### Enable natural scrolling
    $   nvim /etc/X11/xorg.conf.d/XX-touchpad.conf
        Add the option:
        Option "NaturalScrolling" "true"

### Download fonts
    $   cd /usr/share/fonts
    $   wget https://github.com/ryanoasis/nerd-fonts/releases/download/v2.2.2/3270.zip
    $   wget https://github.com/ryanoasis/nerd-fonts/releases/download/v2.2.2/UbuntuMono.zip
    $   wget https://github.com/ryanoasis/nerd-fonts/releases/download/v2.2.2/Mononoki.zip
    $   wget https://github.com/ryanoasis/nerd-fonts/releases/download/v2.2.2/JetBrainsMono.zip
    $   unzip *.zip

### Download qtile configuration:

    Leer el repo antes de clonar
    $   cd ~.
    $   rm -rf qtile
    $   git clone https://github.com/estebenguio/qtile
    

### Instalar nodejs
    $   sudo pacman -S nodejs npm

### Instalar jdk
    $   sudo pacman -S jdk11-openjdk

### Instalar JetBrains
    -   Ir a https://www.jetbrains.com/toolbox-app/
    -   Descargar en formato tar.gz
    $   cd ~/Downloads
    $   tar -zxvf jetbrains-toolbox*.tar.gz
    $   cd jetbrains*
    $   ./jetbrains*
    -   Manage your IDES from here
    
### Instalar brave
    $ sudo pacman -S brave

### Docker
### kubernetes
### 
    
