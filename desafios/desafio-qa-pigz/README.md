# desafio-qa-pigz

Desafio para a vaga de QA na Pigz.

## Regras básicas
1. Você deverá subir este desafio em um repositório público no seu github pessoal ou enviar o arquivo com a solução para o e-mail desafio@pigz.com.br 
2. Para avaliar suas habilidades, gostaríamos que você realizasse os dois desafios.
3. Caso não consiga concluir todos os passos, não se preocupe, nos envie mesmo assim o que você fez para que possamos avaliar.

# Desafio 1

Estamos desenvolvendo um novo sistema de delivery de comida e precisamos de sua ajuda para criar casos de testes que vão validar as funcionalidades do sistema.

**Funcionalidade 1 - Cadastro de novos restaurantes**

Para cadastrar um novo restaurante em nosso sistema, o usuário deve seguir os seguintes passos:

1. Acessar o painel de administração do sistema.
2. Selecionar a opção "Cadastro de restaurantes".
3. Preencher os seguintes campos obrigatórios: nome, endereço (dividido em rua, número, complemento, bairro, cidade, estado e CEP), telefone e CNPJ.
4. O sistema deve validar se o CNPJ informado é válido.
5. Clicar no botão "Salvar".
6. O sistema deve exibir uma mensagem de confirmação e redirecionar o usuário para a lista de restaurantes cadastrados.

**Regras de negócio:**

- O CNPJ é um campo obrigatório e deve ser validado pelo sistema antes do cadastro.
- Não é permitido cadastrar dois restaurantes com o mesmo CNPJ.

**Funcionalidade 2 - Cadastro de cardápios**

Para cadastrar um novo cardápio em nosso sistema, o usuário deve seguir os seguintes passos:

1. Acessar o painel de administração do sistema.
2. Selecionar a opção "Cadastro de cardápios".
3. Selecionar o restaurante desejado.
4. Preencher o nome do cardápio e uma breve descrição.
5. Para cada item do cardápio, preencher os seguintes campos: nome, descrição e preço.
6. Clicar no botão "Salvar".
7. O sistema deve exibir uma mensagem de confirmação e redirecionar o usuário para a lista de cardápios cadastrados.

**Regras de negócio:**

- O nome do cardápio é um campo obrigatório.
- O nome de cada item do cardápio é um campo obrigatório.
- O preço de cada item do cardápio é um campo obrigatório e deve ser um valor válido.
- Não é permitido cadastrar dois cardápios com o mesmo nome para o mesmo restaurante.

Agora que você já sabe as funcionalidades que deverá testar, por favor, elabore um plano de testes manuais para verificar se o sistema está de acordo com as especificações. Lembre-se de usar sua imaginação para visualizar o site e assim mostrar sua capacidade de análise.

Para esse desafio, recomendamos que você siga um padrão de plano de testes ou casos de testes simples. Por exemplo, você pode seguir o seguinte modelo:
|Funcionalidade  | Cenário de teste |Passos|Resultado esperado|
|--|--|--|--| 
|  |  |  |  |


Lembre-se de utilizar uma linguagem clara e coerente na escrita dos testes, para que possam ser entendidos por toda a equipe. Além disso, organize os casos de testes de forma apropriada, para que possam ser executados com facilidade.

# Desafio 2

Nesse desafio, você encontrou um bug no novo sistema de delivery de comida na funcionalidade de cadastro de entregadores. Primeiramente, vou descrever a funcionalidade e as regras de negócio para você entender melhor:

**Funcionalidade: cadastro de entregadores**

1- O usuário acessa a página de cadastro de entregadores.
2- Ele preenche o formulário com as informações do entregador (nome, e-mail, CPF, telefone, placa do veículo, modelo do veículo e foto do veículo).
3- O usuário clica no botão de enviar para finalizar o cadastro.

**Regras de negócio:**

- O nome do entregador deve ter no mínimo 3 caracteres e no máximo 50.
- O e-mail deve ser válido e estar no formato correto (exemplo: teste@teste.com);
- O CPF deve ser válido e não pode já ter sido cadastrado no sistema.
- O telefone deve ter o formato (99) 99999-9999.
- A placa do veículo deve ter o formato AAA-9999 ou AAA9A99.
- O modelo do veículo deve ter no máximo 20 caracteres.
- A foto do veículo é opcional.

Agora, vamos ao bug que você encontrou: ao cadastrar um entregador, o sistema permite que o usuário insira um CPF inválido e finaliza o cadastro normalmente, sem exibir nenhuma mensagem de erro.

Esse bug tem um alto impacto, pois permite que entregadores sem CPF válido possam ser cadastrados no sistema, o que pode afetar a segurança e confiabilidade do serviço. Além disso, esse bug também pode afetar a integração com outras ferramentas, como o sistema de emissão de notas fiscais.

Para relatar esse bug, a equipe utiliza o JIRA como gerenciador de tarefas. Seu desafio é simular a criação de um card no JIRA, incluindo as seguintes informações (imagine que você já anexou as evidências como fotos e vídeos):

**- Descrição do bug.**  
**- Passos para reproduzir o bug.**  
**- Prioridade do bug.**  
**- Possíveis impactos no sistema.**  

**Informações adicionais:**

A equipe de desenvolvimento responsável pelo site é composta por três pessoas: Ana, a desenvolvedora front-end; Bruno, o desenvolvedor back-end; e Carol, a gerente de projeto.

Após a criação do card, é importante notificar o desenvolvedor responsável pela funcionalidade e acompanhá-lo até que o bug seja corrigido e testado. Também é importante comunicar a equipe de gerenciamento de projetos sobre o bug encontrado e seus impactos, para que possam avaliar as prioridades do projeto e as possíveis consequências. Lembre-se de que uma boa comunicação na equipe ajuda a garantir que todos os envolvidos estejam alinhados e trabalhando na mesma direção para entregar um produto de qualidade.

Sendo assim, descreva quais passos você tomaria após a criação do card no JIRA, relate com quem você falaria e de que forma agiria para que o problema encontrado fosse resolvido.
