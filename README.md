# 📡 Portal de Serviços para Provedor de Internet (ISP)

Sistema web desenvolvido para centralizar o atendimento ao cliente da FJ Telecom. O projeto atua como um Hub de Serviços, permitindo autoatendimento e reduzindo a demanda do suporte técnico via telefone.

## 🚀 Funcionalidades Principais

* **Gestão Dinâmica de Planos:** Renderização dos cards de planos e preços via JavaScript (Conceito de Componentes), com área administrativa para alteração de valores em tempo real.
* **Financeiro:** Acesso direto à emissão de 2ª via de boletos.
* **Diagnóstico de Rede:** Página dedicada para teste de velocidade (SpeedTest) proprietário da rede.
* **Cobertura:** Visualização de pontos de atendimento e locais com viabilidade técnica.
* **Downloads:** Links diretos para baixar o App do assinante.

## 🛠 Destaques Técnicos & Arquitetura

### Integração de Comunicação "Serverless"
Para otimizar a infraestrutura e reduzir custos com servidores de e-mail (SMTP/Apache), implementei uma solução baseada em **Intent/Protocol Handlers**:
* **E-mail:** O sistema utiliza requisições diretas (`mailto`) para invocar o cliente de e-mail nativo do usuário (Outlook, Gmail App, etc), garantindo entrega imediata sem necessidade de backend intermediário.
* **WhatsApp:** Integração direta com a API de deep linking do WhatsApp para abertura de chat com o suporte.

### Manipulação de DOM
O sistema não depende de HTML estático para os preços. Um script popula o DOM dinamicamente, facilitando a manutenção: basta alterar o objeto de dados para que todos os planos no site sejam atualizados instantaneamente.

## 💻 Tecnologias
* HTML5 & CSS3 (Responsivo)
* JavaScript (ES6+)
* Integrações de API externas (Maps, SpeedTest)
