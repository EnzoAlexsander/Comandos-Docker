# DOCKER

Comandos Docker

sudo*

docker ps = Verificar o status do container

docker ps -a = Lista todos os containeres

docker stats "id container" = Verificar informações sobre um container específico
(ctrl+c = sair do docker stats)

docker inspect "id container" = Informações mais detalhadas sobre a sua imagem ou seu container

docker rmi "nome da imagem" = Deletar uma imagem

docker exec "id container" = Executa qualquer comando no container sem precisar estar no console dele.

	-i = permite interagir com o container
	-t = associa o seu terminal ao terminal do container
	-it = é apenas uma forma reduzida de escrever -i -t
	--name "algum nome" = permite atribuir um nome ao container em execução
	-p 8080:80 = mapeia a porta 80 do container para a porta 8080 do host
	-d = executa o container em background
	-v /pasta/host:/pasta/container = cria um volume '/pasta/container' 		dentro do container com o conteúdo da pasta '/pasta/host' do host

docker images = Listar as imagens que estão no host

docker search "parametro" = Buscar uma imagem. 

docker exec "id container" mkdir /temp/ = Criar um novo diretório dentro do Container sem precisar entrar nele

docker attach "id container" = Entrar dentro do container.

docker start "id container" = Subir um container.

docker stop "id container" = parar um container em execução

docker run "id container" = executar um container

docker run -it ubuntu /bin/bash = Subir o container com o ubuntu e entrar no bash (um exemplo)

docker run --name ubuntinho ubuntu = Exemplo de como dar um apelido ao container.

docker rm "id container" = Remover o container.

docker run -it -p 8080:80 ubuntu = Mapear uma porta para o Container

docker logs "id container" = Para ver todos os comandos executados dentro de um container em execução.
