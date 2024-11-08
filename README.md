Fake Shop - Projeto de Monitoramento e CI/CD

Cenário

O ecommerce Fake Shop está em produção, porém enfrentando dificuldades significativas no processo de entrega e manutenção. Atualmente, o deploy no Kubernetes é muito demorado, exigindo uma mobilização de equipes por até dois dias para cada atualização. Além disso, a ausência de monitoramento deixa a empresa no escuro quanto à disponibilidade da aplicação, só percebendo problemas quando o cliente entra em contato.

Este projeto visa resolver esses problemas implementando uma pipeline de CI/CD para agilizar o deploy e adicionando monitoramento de métricas para garantir a visibilidade do estado da aplicação e do cluster.

Etapas do Projeto

1. Criação de Pipeline CI/CD

Foi desenvolvida uma pipeline de CI/CD usando GitHub Actions para automatizar o processo de deploy. A pipeline realiza a construção da imagem Docker e faz o deploy no cluster Kubernetes, reduzindo o tempo e o esforço necessários para cada atualização de versão.

2. Monitoramento da Aplicação

Para garantir visibilidade sobre a saúde da aplicação e do cluster, foi realizado o deploy do Prometheus e do Grafana no ambiente Kubernetes. Esses componentes permitem monitorar métricas essenciais, como uso de recursos e disponibilidade da aplicação.

Pasta Grafana

Todos os prints das métricas estão disponíveis na pasta grafana, localizada neste repositório. Eles mostram o monitoramento da aplicação e do cluster, evidenciando o funcionamento do sistema de alerta em tempo real.

Conclusão

Este projeto permite uma maior eficiência no processo de deploy e monitoramento do Fake Shop, facilitando a detecção de problemas e reduzindo o tempo de resposta.
