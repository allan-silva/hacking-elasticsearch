# hacking-elasticsearch
Algumas informações para facil compartilhamento entre máquinas, para rodar o elastic e debugar via IDE


Rodar:  
`./gradlew :run`

Alterar Senha dos usuários:  
`export ES_PATH_CONF=/home/allan-silva/code.allan/elasticsearch/build/testclusters/runTask-0/config`  

`/home/allan-silva/code.allan/elasticsearch/distribution/archives/linux-tar/build/install/elasticsearch-8.0.0-SNAPSHOT/bin/elasticsearch-setup-passwords interactive`  


DEBUG MODE:  

Inciciar o deug server, pelo menu "Debug Elasticsearch"  
Iniciar a execução com: `./gradlew run --debug-jvm`


Criar indice:  
`PUT {{elastic}}/my-index`  
Entrypoint: `server/src/main/java/org/elasticsearch/rest/action/admin/indices/RestCreateIndexAction.java`  
`org/elasticsearch/action/support/master/TransportMasterNodeAction.java:150`  
`org/elasticsearch/indices/cluster/IndicesClusterStateService.java:225`  
`org/elasticsearch/indices/IndicesService.java:539`  
