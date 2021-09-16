
INSTALLATION DE VUE JS

### STEP 1
    Installation de Node Js  (npm )
    -sudo apt install nodejs
    -nodejs -v

### STEP 2 
    Installation de npm
    -sudo apt install npm
    -npm -v


### STEP 3
    Installation de Yarn
    -curl -sS https://dl.yarnpkg.com/debian/pubkey.gpg | sudo apt-key add -
    -echo "deb https://dl.yarnpkg.com/debian/ stable main" | sudo tee /etc/apt/sources.list.d/yarn.list

### STEP 4
    mettre a jour la list des package
    -sudo apt update
    -sudo apt install yarn
    -yarn --version
    

### STEP 5
    Installation de vue js 
    - npm install vue
    -yarn global add @vue/cli
     #OR
    -npm install -g @vue/cli

    Updrate
    -npm update -g @vue/cli
    # OR
    -yarn global upgrade --latest @vue/cli

