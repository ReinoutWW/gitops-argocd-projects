microk8s helm3 repo add itzg https://itzg.github.io/minecraft-server-charts

microk8s helm3 repo update

microk8s helm3 install minecraft itzg/minecraft   --namespace minecraft   --create-namespace   -f values.yaml --set minecraftServer.eula=true