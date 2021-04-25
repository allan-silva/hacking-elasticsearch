# hacking-elasticsearch
Algumas informações para facil compartilhamento entre máquinas, para rodar o elastic e debugar via IDE


Rodar:  
`./gradlew :run`

Alterar Senha dos usuários:  
`export ES_PATH_CONF=/home/allan-silva/code.allan/elasticsearch/build/testclusters/runTask-0/config`  

`/home/allan-silva/code.allan/elasticsearch/distribution/archives/linux-tar/build/install/elasticsearch-8.0.0-SNAPSHOT/bin/elasticsearch-setup-passwords interactive`  

Criar indice:  
`PUT {{elastic}}/my-index`  

