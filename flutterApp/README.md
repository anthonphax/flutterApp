#Atividade  

## Execução do projeto
 ``flutter pub get`` 

``flutter run`` 

``flutter run -d chrome``

Roteiro da atividade

Sugestão: para não deixar tudo acumulado para o final, sugere-se fazer cada uma das etapas por semana, para no final realizar uma única entrega.
Utilizar como base a versão do projeto disponível no repositório:
https://github.com/matsunagasistemafiep/flutter_app_2023/tree/unisenai

Etapa 1

    1) Alterar o ícone do Aplicativo e o nome do aplicativo com o padrão: SEU_NOMEApp (No lugar do SEU_NOME, usar seu primeiro nome). Com relação ao ícone, fica livre para cada um definir como quiser. Sugere-se utilizar o link para gerar o ícone. Para alterar o ícone, siga as instruções do Readme disponível no link do repositório.
    2) Crie uma tela ou utilize a tela de perfil já existente (com os forms) contendo dados do perfil do usuário. Esta tela deve conter campos como nome, CPF, e-mail, telefone, data de nascimento e uma foto de perfil. A tela deve permitir editar e salvar os dados do perfil no sharedPreferences (base de dados local). A foto de perfil pode ser modificada utilizando a biblioteca image_picker, podendo ser mudada por câmera ou uma imagem da galeria, conforme o exemplo da versão atual. 
    3) Adicione um botão perto da de salvar, chamado “enviar e-mail”. Este botão deve permitir abrir um app de envio de e-mail para o e-mail digitado no formulário. Utilize o url_launcher para isso.

Etapa 2

    1) Crie uma tela contendo um campo de texto simples, que consiste em um campo para o usuário digitar o CEP. Em seguida, após digitar o CEP, deve ter um botão para buscar o CEP digitado. Você deve utilizar uma conexão via API que retorna os dados do CEP. Utilize como base o exemplo desenvolvido no projeto da Pokedex - https://github.com/ftakematsu/pokemon_flutter_app 
A API é: https://viacep.com.br/ws/01001000/json/
No lugar do 01001000 deve conter o CEP digitado. Em seguida o retorno será um JSON:
   {
      "cep": "01001-000",
      "logradouro": "Praça da Sé",
      "complemento": "lado ímpar",
      "bairro": "Sé",
      "localidade": "São Paulo",
      "uf": "SP",
      "ibge": "3550308",
      "gia": "1004",
      "ddd": "11",
      "siafi": "7107"
    }
Com base nisso:
        a. Crie uma classe (Model) que represente o CEP. Utilize a arquitetura services -> repositories, conforme o exemplo da Pokedex. Quando a API do CEP for chamada, deve-se gerar um objeto da classe contendo os dados buscados do JSON. 
        b. Após o CEP ser buscado, a tela deve exibir as informações completas do endereço.

    2) Crie um botão logo abaixo que abra, via URL Launcher, um link do Google Maps que abra o mapa para o endereço localizado, abrindo o aplicativo do Maps para o endereço passado. Para isso, basta abrir via url_launcher, a URL seguindo o modelo abaixo:
        a. https://www.google.com.br/maps/place/Rua+Belem+844 

    3) Com o recurso de geolocalização, busque o endereço atual por meio do GPS, utilizando os métodos já implementados no projeto. Em seguida, se o endereço localizado pelo GPS for igual ao endereço buscado pelo CEP, mostrar uma mensagem em forma de modal dizendo: “Você está na mesma localização do CEP digitado”.


Etapa 3

    1) Faça melhorias no design da aplicação de modo geral – utilize a sua criatividade para esta etapa. Pode melhorar questões de layout, cores, fontes, tamanho, inclusão de caixas de notificação, splash, loadings de carregamento quando necessários, dentre outros recursos. Se necessitar, pode instalar novas bibliotecas e recursos.

    2) Gere o build da aplicação, isto é, o APK do aplicativo e envie no AVA. Como o tamanho do arquivo normalmente é grande, sugere-se salvar o arquivo em uma pasta na nuvem (One Drive, Google Drive, etc) e enviar o link. Para gerar o build, execute o comando flutter build apk. 

Possíveis formas de entrega:
    • Arquivos-fonte do projeto zipados.
    • Pasta do projeto compartilhado em um armazenamento em nuvem.
    • Repositório do GitHub.