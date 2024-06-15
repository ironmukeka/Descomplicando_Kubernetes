# Comandos úteis

Utilizando o WSL2 no Windows 11, tive problemas para deployar PODs no cluster criado pelo kind. 
Para normalizar após uma pesquisa nas internets, encotrei o know-how abaixo.

> Caso o kind não consiga iniciar as imagens direto seguir os passos abaixo:
- Executar o docker pull da imagem 
- Executar o load da imagem no kind
- Executar o kubectl run com o nome da imagem que você baixou

```Shell
docker pull nginx
kind load docker-image nginx:latest
kubectl run nginx --image nginx:latest
```
