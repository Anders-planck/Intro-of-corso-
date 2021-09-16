Installer Zsh sur sa macchine pour facilite l usage du terminale et
rendre le terminal umpe plus attreant en codant


STEP 1
    - tape dans le terminal 
    sudo apt install zsh

STEP 2
    apres l installation complete de zsh .par defaut la shell ne se demare pas 
    automatiquement sur Zsh mais sur bash et pour y remedier , taper cette 
    commande dans le terminal
    -echo $SHELL (pour verifier quelle est le moteur par defaut de votre shell)
    
    Dans le cas ou votre shell ne demare pas sur bash alors taper cette commande
    - (sudo) chsh -s $(which zsh)

STEP 3

    installation et Configuration de Zsh

    STEP 3.1
    Avant tout nous ne  devons pas oublier d intaller  des extension qui nous permetrons 
    de telecharge du terminal la dernier version de zsh et l installer (curl ou wget ) 
    et aussi (git) qui nous permettra d interagir avec github.
    taper la commande: -sudo apt install curl wget git

    STEP 3.2
    telechargement et installation de Zsh
    -sh -c "$(curl -fsSL https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"
    or 
    -sh -c "$(wget -O- https://raw.githubusercontent.com/ohmyzsh/ohmyzsh/master/tools/install.sh)"


STEP 4 

    Changement du theme par defaut de zsh.
    le theme par defaut de zsh est robbyrusell.
    pour changer cette Configuration par defaut on devra editer le fichier .zshrc

    STEP 4.1
    Taper dans  le  terminal ces 2 commandes:

    -cd ~/.oh-my-zsh/themes/  (pour acceder au dossier themes de zsh)
    -ls -a (pour lister l ensemble d element contenue dans la cartella )

    STEP 4.2
    Installation de quelque librerie pour l installation du theme "zsh-multiline"

    -git clone https://github.com/jan-auer/zsh-multiline.git ~/.oh-my-zsh/custom/themes/zsh-multiline


    STEP 4.3 

    Edition du fichier .zshrc

    taper dans le terminal:
    -vi ~/.zshrc

    (
        si part defaut vous n avez pas vi preinstaller dans votre ordinateur 
        taper la commande si dessous pour  l'installer :
        -sudo apt update (pour mettre a jour tout les packages  deja telechager)
        -sudo apt install vim
        -vim --version (juste pour verifier que tout c est bien installer)
    )

    - ZSH_THEME="zsh-multiline/multiline" ou "agnoster" (changer dans le  fichier .zshrc) 

    -source ~/.zshrc (pour relancer zsh)

    STEP 4.4
    Apres tout ceux ci faudra installer la powerline fonts pour mettre a jour et telecharger les  icons donc le theme a besion pour fonctioner

    -sudo apt-get install powerline fonts-powerline

    STEP 4.5

    pour ne plus afficher le username editer a nouveau le fichier .zshrc

    -DEFAULT_USER=$USER

STEP 5

    ACtiver certain plugins pour rendre plus performant zsh
    -cd ~/.oh-my-zsh/plugins/
    -ls -a

    STEP 5.1
    Telechargement des plugins necessaire
    -git clone https://github.com/zsh-users/zsh-autosuggestions.git $ZSH_CUSTOM/plugins/zsh-autosuggestions

    -git clone https://github.com/zsh-users/zsh-syntax-highlighting.git $ZSH_CUSTOM/plugins/zsh-syntax-highlighting 

    STEP 5.2
    editer a nouveau le fichier .zshrc 
    -vi ~/.zshrc
    -plugins=(git zsh-autosuggestions zsh-syntax-highlighting)
    -source ~/.zshrc


STEP 6 
    DEsintallation de zsh
    -uninstall oh_my_zsh




    














STEP Final au cas ou yas des soucis 
- aller sur le site:
https://qirolab.com/posts/install-and-setup-oh-my-zsh-on-ubuntu-system
pour suivre les etape de  l installation pas a pas 

