# HTML conteiner 

Exemplo de conteiner docker com html + nginx. 

## Como utilizar para teste. 

    docker-compose up --build

Ao moduficar a pasta ./Public irá refletir automaticamente na porta 8080.

# Colocar em produção

Para colocar em produção temos que tirar a versão teste e subir a versão de produção que não tem live-reload como a versão teste.

## Tirando a versão de teste.

    docker-compose down

## Subindo a versão de produção

    docker-compose -f docker-compose-prod.yml up --build    

Pronto agora a aplicação está rodando na porta 80