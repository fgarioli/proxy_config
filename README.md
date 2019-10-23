# Configuração de Proxy

### npm

- `$ npm config set proxy http://[user]:[password]@[proxy]:[port]`

 `$ npm config set http-proxy http://[user]:[password]@[proxy]:[port]`

- `$ npm config set https-proxy http://[user]:[password]@[proxy]:[port]`

- `$ npm config set registry http://registry.npmjs.org/`

- `$ npm set strict-ssl false`

Arquivo .npmrc (exemplo):

    proxy=http://[user]:[password]@[proxy]:[port]
    http-proxy=http://[user]:[password]@[proxy]:[port]
    https-proxy=http://[user]:[password]@[proxy]:[port]
	registry=http://registry.npmjs.org
    strict-ssl=false

### git

- `$ git config --global http.proxy http://[user]@[proxy]:[port]`

- `$ git config --global credential.helper wincred`

Arquivo .gitconfig (exemplo):
#### 
    [user]
        name = Fernando Garioli
        email = f.ribeirogarioli@gmail.com
    [http]
        proxy = http://[usuario]@[proxy]:[port]
    [https]
        sslVerify = false
        proxy = https://[usuario]@[proxy]:[port]
    [credential]
        helper = wincred

**Obs.: ambos os arquivos ficam no diretório do usuário.**