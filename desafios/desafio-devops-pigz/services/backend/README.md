
# Back end php (symfony)

Este desafio é focado em aplicação back end, aqui estar o passo a passo de como realizar.

# Requisitos para desafio

1. Ferramentas como docker e docker-compose
2. PHP 7.4 e composer (opcional ambos)
3. VS Code ou editor de código
4. Github CI

## Como realizar o desafio

### DockerFIle e docker-compose
Esses arquivos estão vazios, analise esse passo a passo como é feito manualmente o build e levantar servidor e adapta para DockerFile. Crie os containers que use nginx e outro de php-fpm como mostrado nos arquivos necessários

#### Passos:
1. Instalar pacotes necessários do projeto via apt install como php-xml
2. Composer install (instalação dos pacotes do projeto)
3. Mover os codigos no docker/nginx para /var/www/app que será utilizado 
4. Mover os arquivos docker/nginx/default.conf no docker/nginx para locais de configuracao do nginx

#### Considerações:
1. O DockerFile ja tem imagens docker pre-setadas, como imagem do nginx e php-fpm. Na imagem do php-fpm nao tem composer pré instalado
2. O docker-compose ja tem uma arquitetura de build ja feita com nomes e tals, porem quero que exponha as portas e cria volume para nginx tenha acesso ao php-fpm.sock

### Github CI
Se você conseguiu terminar dockerfile, docker-compose e deu docker-compose up ai finalmente conseguiu levantar servidor e apareceu tela `Welcome to Symfony`, agora estar pronto para proximo passo.

#### Passos:
1. Procurar forma de fazer build via actions do github
2. Fazer build e enviar para docker hub com suas credenciais ( opcional mas desejável )
3. Conseguir funcionar até botão ficar verde
4. Manda o link do repositório para a gente verificar

Boa sorte e divirta-se!
