# desafio-qa-pigz

Desafio para a vaga de DevOps na Pigz. Este desafio é voltado para candidatos iniciantes na área, não sendo necessário conhecimento prévio das linguagens utilizadas nos projetos. O objetivo é consultar o README para aprender sobre o processo de build e aplicá-lo no CI do Github Actions ou na plataforma de sua preferência.

## Regras básicas
1. Você deverá subir este desafio em um repositório público no seu github pessoal ou enviar o(s) arquivo(s) com a solução para o e-mail desafio@pigz.com.br 
2. Caso não consiga concluir todos os passos, não se preocupe, nos envie mesmo assim o que você fez para que possamos avaliar.

# Requisitos para desafio

1. Ferramentas como docker e docker-compose
2. Conhecimento básico de lógica de programação e sistemas
3. Link do projeto para realizar o desafio:
	* Back end: [Projeto php symfony](./services/backend)
4. Plataforma de CI/CD (Github Actions)


## Como realizar o desafio

### Sistema a ser executado (olhar na pasta service e escolhe um)
Uma aplicação desenvolvida em PHP utilizando o framework Symfony. A aplicação deve ter um build de Docker e ser automatizada com CI/CD.

#### Passos:
1. Com base no README.md, que contém todos os passos para realizar o build, crie um Dockerfile.
2. Crie um arquivo docker-compose.yml baseado no diagrama presente no README.md.
  * Por exemplo, se for o backend, o docker-compose deve subir um banco de dados e o Redis. No frontend, deve-se criar uma fake API com JSON.
3. Implemente, por meio do CI, o passo a passo para realizar o build do Docker e enviar para o Docker Hub a cada commit enviado ao repositório.
4. Nos arquivos Dockerfile, docker-compose.yml e outros que você criar, faça comentários documentando o que foi feito e o que entendeu (opcional).

### O desafio será avaliado com base em:
* Funcionalidade da automação do build;
* Conhecimento das ferramentas e como foram utilizadas;
* Funcionalidade e qualidade do seu código;
* Os itens opcionais não são obrigatórios.

Boa sorte e divirta-se!
