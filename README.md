# devopsTools

<h1> Devops Tools </h1>
<br>
<h2> Ferramentas </h2>
<h3>Rancher, K8s, Docker, AWS, Traefik DNS...</h3>
<br>
<h4> Em andamento </h4>

<h3> Esse repositorio armazena arquivos de configurações devops para desenvolvimento continuo </h3>

<br>

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
<h4>...</h4>