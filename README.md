<h1> Devops Tools </h1>
<br>
<h2> Ferramentas </h2>
<h3>Rancher, K8s, Docker, AWS, Traefik DNS...</h3>
<br>

<h3> Esse repositorio armazena arquivos de configurações devops para desenvolvimento continuo, com a finalidade de orquestrar clusters K8s através do Rancher, o ambiente foi criado em cloud na AWS.</h3>

<h4>Abra a o jpg "LLD" para consultar o low level design da infra</h4>

<br>

<h3>Files</h3>
<h4>ui.yml = Arquivo responsavel por configurar o DNS em que o Traefik ira responder</h4>
<br>
<h4>configmap.yml = setar configurações dos  serviços externos aos contâiners que estão rodando a aplicação </h4>
<br>
<h4>secrets.yml = Os secrets são responsaveis salvar dados sensiveis dentro do Cluster, como por exemplo, senhas do banco de dados</h4>
<br>
<h4>liveness.yml =  liveness é responsavel por verificar se a aplicação esta rodando, caso a aplicação não responda ela é finalizada e criada em em outro node</h4>
<br>
<h4>rolling-udpate.yml = com o rolling-update, conseguimos atualizar as imagens em produção, substintuindo por uma imagem atualizada sem interrupções no sistema</h4>
<br>
<h4>php-apache.yml = serviço criado para stress test no processador</h4>
<br>
<h4>hpa.yml = cria um serviço de auto-escalonamento para o serviço php-apache.yml</h4>
<br>
<h4>node-selector.yml = adicionamos a função node selector no pod, assim ele so pode rodar em pods com a tag definida no "node-selector.yml"</h4>
<br>
<h4>pipeline-rancher-k8s/Dockerfile = Arquivo de build do docker</h4>
<br>
<h4>pipeline-rancher-k8s/.rancher-pipeline.yml = Pipeline Jenkins-Rancher configurado</h4>
<br>
<h4>pipeline-rancher-k8s/deployment.yml = Função de deploy chamada por ".rancher-pipeline.yml" para terminar o pipeline</h4>
<br>
<h4>pipeline-rancher-k8s/main.go = Aplicação API go</h4>
<br>
<h4>function-nodejs.yml = yaml para executar funções kubeless, função python criada.</h4>
<br>
<h4>network-policy.yml = yml para politica de rede, define comunicação dos pods </h4>
<br>
<h4>cpu-contraints.yml = yml para definir parametros de uso de cpu por namespace</h4>
<br>
<h4>cpu-contraints-pod.yml = deploy de pod para teste dos parametros de cpu "cpu-contraints.yml", parametros de CPU OK</h4>
<br>
<h4>cpu-contraints-pod-2.yml = deploy de pod para teste dos parametros de cpu "cpu-contraints.yml", parametros de CPU NOT OK</h4>
<h4></h4>
<h5>Em andamento</h5>