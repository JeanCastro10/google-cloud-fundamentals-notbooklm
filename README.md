# google-cloud-fundamentals-notbooklm
Estudos e projetos práticos em Google Cloud Platform, abrangendo infraestrutura (VPC, VMs), segurança (IAM) e arquiteturas Cloud Native e Serverless


 
Contexto e Objetivos

O propósito deste repositório é consolidar o conhecimento sobre as soluções de computação em nuvem providas pelo Google, focando em performance de aplicações, infraestrutura e segurança

Objetivos de Estudo:
Reconhecer os diferenciais dos serviços do Google Cloud (GCP) em relação ao modelo tradicional on-premises


Dominar a configuração de infraestrutura elástica e aplicações Cloud Native


Identificar e aplicar as melhores práticas de segurança (IAM) e operações (SRE/DevOps) em ambientes de nuvem

2. Curadoria de Fontes
Para compor este estudo, foram selecionadas fontes que abrangem desde a base teórica até a aplicação prática:
Fonte 1: Fundamentos e Modelos de Serviço: Explora as diferenças entre IaaS, PaaS e SaaS e o modelo de responsabilidade compartilhada

Fonte 2: Infraestrutura de Redes (VPC): Detalha o funcionamento da rede global do Google e o uso de subnets para baixa latência

Fonte 3: Computação e Máquinas Virtuais: Guia sobre o uso do Compute Engine e a escolha de famílias de máquinas (E2, N2, C2)

Fonte 4: Arquiteturas Modernas: Focada em soluções Serverless (Cloud Run) e mensageria assíncrona (Pub/Sub)

Fonte 5: Estudo de Caso TechNova: Um cenário prático de troubleshooting para resolver problemas de latência e segurança em uma startup

3 Engenharia de Prompts e "Cicatrizes"
Nesta seção, você deve documentar como interagiu com a IA para extrair o conteúdo.
Prompt Estratégico: "Considere a situação da TechNova e proponha soluções para otimizar redes e garantir a segurança".
Resultado: A IA conectou o conceito de VPC Global com a necessidade de reduzir latência regional

"Cicatriz" (Troubleshooting): Durante o estudo, uma dificuldade encontrada foi identificar a lista exata de produtos do Free Tier, pois as fontes mencionavam sua existência para estudo, mas não listavam os nomes nominais (como BigQuery ou Cloud Storage), o que exigiu uma busca externa complementar

4. Miniguia de Estudo (Entrega Final)
Resumo Estruturado
A computação em nuvem no GCP funciona como um aluguel de recursos (CPU, memória e rede) sob demanda
 A infraestrutura é organizada em Regiões e Zonas, conectadas por uma rede privada de cabos submarinos, garantindo alta disponibilidade
 O sucesso de uma migração depende de adotar uma arquitetura Cloud Native, preferencialmente Stateless, para permitir escalabilidade automática e redução de custos

Glossário de Conceitos
VPC (Virtual Private Cloud): Rede virtual privada global onde os recursos são isolados e configurados

IAM (Identity and Access Management): Gestão de permissões para garantir que cada usuário acesse apenas o necessário

Compute Engine: Serviço de IaaS para criação e gestão de máquinas virtuais

Cloud Run: Plataforma PaaS para execução de containers de forma serverless

Pub/Sub: Serviço de mensageria para comunicação assíncrona entre sistemas

Prompts Reutilizáveis para Revisão
"Explique a diferença entre uma arquitetura Stateful e Stateless no contexto de escalabilidade do Cloud Run."

"Quais são as 6 camadas de segurança física dos datacenters do Google?"
.
"Como a matriz de responsabilidade compartilhada muda ao migrar de Compute Engine (IaaS) para Cloud Run (PaaS)?"
