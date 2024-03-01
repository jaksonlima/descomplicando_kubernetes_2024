# Descomplicando Kubernetes 2024

[https://kubernetes.io/]

## Instalação kubectl

[https://kubernetes.io/docs/tasks/tools/install-kubectl-linux/]

# Meu .bashrc linux Ubuntu referente ao Docker e kubectl

```
#ALIAS KUBECTL
alias k="kubectl"

#ALIAS DOCKER
alias d="docker"

#BASH_COMPLETION, USADO TAMBÉM PARA KUBECTL AUTO COMPLETE
source /usr/share/bash-completion/bash_completion
source <(kubectl completion bash)
complete -o default -F __start_kubectl k
```
