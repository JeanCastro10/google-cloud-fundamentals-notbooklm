# google-cloud-fundamentals-notbooklm
Estudos e projetos práticos em Google Cloud Platform, abrangendo infraestrutura (VPC, VMs), segurança (IAM) e arquiteturas Cloud Native e Serverless


 
☁️ Jornada Google Cloud: De Fundamentos à Arquitetura Cloud Native
Este repositório contém meu caderno de estudos e projetos práticos sobre Google Cloud Platform (GCP). O material explora como a computação em nuvem transforma a infraestrutura física em tecnologia como serviço, permitindo escalabilidade global, alta disponibilidade e segurança robusta.
🎯 Contexto e Objetivos
A migração para a nuvem não é apenas uma mudança de servidor, mas uma mudança de paradigma. O objetivo deste estudo é dominar as ferramentas do Google Cloud para resolver desafios reais de negócios, como latência global e picos de tráfego, utilizando a analogia central de que a nuvem funciona como um aluguel de recursos (CPU, memória e rede), onde a manutenção física é responsabilidade do provedor

Objetivos principais:
Compreender os modelos de serviço (IaaS, PaaS, SaaS) e a Matriz de Responsabilidade Compartilhada

Dominar a infraestrutura global: Regiões, Zonas e Redes VPC

Explorar arquiteturas Cloud Native e Serverless para otimização de custos e performance


--------------------------------------------------------------------------------
📚 Curadoria de Fontes
Para este estudo, utilizei uma curadoria de 32 fontes, incluindo documentos técnicos e transcrições de aulas com o Professor Iago Leone. As principais referências foram:
Fundamentos de Cloud: Transcrições sobre a história e conceitos básicos (IaaS vs PaaS vs SaaS)

Infraestrutura de Rede: Documentação sobre VPCs globais e subnets regionais

Computação e VMs: Guia sobre Compute Engine e famílias de máquinas (E2, N2, C2)

Segurança e IAM: Material focado em Identity and Access Management e proteção contra ataques (Cloud Armor)

Aplicações Modernas: Estudo sobre arquiteturas Stateless, Serverless (Cloud Run) e Mensageria (Pub/Sub)


--------------------------------------------------------------------------------
🧠 Engenharia de Prompts e "Cicatrizes"
Abaixo, registro o processo de interação com a IA (NotebookLM) para consolidar o conhecimento.
Pergunta Estratégica (Prompt):
"A startup TechNova está enfrentando problemas de latência entre regiões e quedas em horários de pico. Como o Google Cloud pode resolver isso utilizando subnets e comunicações assíncronas?"
Raciocínio Técnico (A "Cicatriz"): Um dos maiores desafios no aprendizado foi entender que a VPC do Google Cloud é global
. Diferente de outros provedores, você pode criar uma rede que abrange o mundo todo, mas deve alocar as subnets regionalmente para reduzir a latência via geolocalização
. Além disso, a solução para os picos de tráfego não foi apenas "aumentar a máquina", mas adotar o Pub/Sub para desacoplar sistemas, garantindo que o checkout não trave se o sistema de nota fiscal falhar (comunicação assíncrona)


--------------------------------------------------------------------------------
🚀 Miniguia de Estudo (Entrega Final)
1. Resumo Estruturado: O Ecossistema GCP
Modelos de Serviço: No IaaS (Compute Engine), você cuida do SO e da aplicação
. No PaaS (Cloud Run), você foca apenas no código
. No SaaS (Gmail), você apenas consome o serviço

Infraestrutura: O Google utiliza uma rede privada de cabos submarinos
. Para alta disponibilidade, os recursos devem ser distribuídos em diferentes Zonas (a, b, c) dentro de uma Região

Segurança: A segurança física tem 6 camadas nos datacenters
. Virtualmente, o IAM garante que cada usuário tenha o acesso mínimo necessário (Princípio do Menor Privilégio)

2. Glossário de Conceitos Chave
VPC (Virtual Private Cloud): Rede virtual privada e segura para conectar seus recursos

Cloud Run: Serviço PaaS para rodar containers de forma Serverless e escalável

Pub/Sub: Ferramenta de mensageria para permitir que sistemas conversem sem estarem "sincronizados"

IAM (Identity and Access Management): Gestão de quem pode fazer o quê em cada recurso

Cloud Native: Aplicações desenhadas para serem leves, elásticas e econômicas na nuvem

3. Caso Prático: Solução TechNova
Para a startup fictícia estudada, a arquitetura proposta incluiu:
Subnets Regionais: Redução de latência atendendo usuários pelo servidor mais próximo

Arquitetura Stateless: Uso de Cloud Run para escalar de 1 a 1 milhão de usuários instantaneamente

Segurança Robusta: Implementação de MFA (Autenticação de Múltiplos Fatores) e Cloud Armor para mitigar ataques DDoS

4. Prompts de Revisão (Prontos para Uso)
"Explique a diferença de responsabilidade de segurança entre uma VM e o Cloud Run."
"Como o uso de uma arquitetura sem estado (Stateless) ajuda a economizar dinheiro no Google Cloud?"
"Quais métricas o Cloud Monitoring deve coletar para prever quedas de sistema?"

