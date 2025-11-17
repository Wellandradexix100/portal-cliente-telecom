# 📡 Portal de Serviços & Autoatendimento ISP

Sistema web desenvolvido para a FJ Telecom, atuando como um Hub central de serviços, financeiro e suporte técnico automatizado. O projeto foca na experiência do usuário (UX) para reduzir a demanda do call center através de ferramentas de autoatendimento.

## 🚀 Funcionalidades Principais

### 🛠 Painel do Cliente & Serviços
* **Gestão Dinâmica de Planos:** Renderização dos cards de planos via JavaScript, com painel administrativo oculto para alteração de preços e nomes em tempo real.
* **Financeiro:** Emissão rápida de 2ª via de boletos.
* **Diagnóstico de Rede:** SpeedTest proprietário integrado.
* **Cobertura:** Mapa interativo de viabilidade técnica e Pontos de Presença (PoPs).

### 📚 Base de Conhecimento (Troubleshooting)
Focado na redução de chamados de nível 1 (N1):
* **Guia de Solução de Falhas:** Tutoriais interativos para problemas comuns (ex: travamento de roteador, verificação de cabos).
* **Onboarding de Streaming:** Passo a passo para o cliente configurar e acessar o serviço de mídia (Emby FJ Telecom).
* **Conteúdo Educativo:** Área de vídeos e blog integrado para educação do usuário.

### 📢 Mídia & Engajamento
* **Galeria Visual:** Exibição dos pontos físicos e estrutura da empresa.
* **Integração Social:** Feed e destaques de postagens do Instagram.

## 🛠 Destaques Técnicos

### Integração "Serverless" para Comunicação
Utilização de **Protocol Handlers** para integrar e-mail e WhatsApp:
* O sistema invoca diretamente os clientes de e-mail e APIs de mensagem do dispositivo do usuário, garantindo comunicação instantânea sem a complexidade/custo de manutenção de servidores SMTP dedicados.

### Arquitetura Orientada a Componentes (Vanilla JS)
Apesar de não utilizar frameworks pesados, a estrutura do código segue o princípio de componentes:
* Dados dos planos isolados em objetos JSON.
* Renderização do DOM feita via loops e injeção de templates, permitindo atualizações globais de interface apenas alterando a fonte de dados.

## 💻 Tecnologias
* HTML5 & CSS3 (Design Responsivo)
* JavaScript (ES6+)
* Integração com serviços de Streaming (Emby)
* APIs de Mapas e Redes Sociais
