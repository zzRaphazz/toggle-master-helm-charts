# Charts Helm — ToggleMaster

Não havia charts Helm de aplicação no monorepositório de origem; portanto, este repositório é um scaffold inicial, não uma conversão de deploy existente.

Os workloads atuais dos serviços são gerenciados como manifests Kustomize em `toggle-master-k8s-manifests`. Não adicione releases Helm para os mesmos recursos sem migrar explicitamente a responsabilidade; Argo CD/Helm e manifests puros não devem gerenciar simultaneamente os mesmos objetos Kubernetes.

Adicione aqui charts revisados e versionados quando um componente gerenciado por Helm for escolhido. Mantenha as Applications do Argo CD e a configuração de bootstrap em `toggle-master-argocd-config`. Não copie charts de terceiros para este repositório; use os repositórios publicados com versões fixas e armazene somente values/configuração próprios do projeto quando apropriado.
