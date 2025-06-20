# DIO - Monitoramento no Azure: Visão geral e Exemplo

O monitoramento no Azure é uma prática essencial para organizações que dependem da infraestrutura em nuvem para suas aplicações e serviços. A Microsoft oferece um conjunto de ferramentas de monitoramento, tendo o Azure Monitor como plataforma central. O Azure Monitor coleta e analisa dados de telemetria de uma ampla variedade de recursos do Azure, como máquinas virtuais (VMs), bancos de dados e componentes de rede.

Principais recursos do monitoramento no Azure:

Métricas e Logs: O Azure Monitor coleta métricas de desempenho e logs de diagnóstico dos recursos, fornecendo insights sobre a saúde e o uso deles.
Alertas: É possível configurar alertas baseados em condições específicas. Quando um alerta é disparado, o Azure pode notificar você por e-mail, SMS ou até acionar ações automatizadas.
Painéis e Visualização: Os painéis centralizados permitem a visualização em tempo real do estado dos seus recursos.
Integração: O monitoramento do Azure se integra a outras ferramentas de segurança e gerenciamento do Azure, garantindo conformidade e resposta rápida a incidentes.
Exemplo de Cenário: Exclusão de uma Máquina Virtual e Recebimento de Alerta

Suponha que você deseje monitorar recursos críticos para evitar exclusões acidentais ou alterações não autorizadas. No Azure, é possível configurar um Alerta de Log de Atividades para ser notificado sempre que uma ação específica—como a exclusão de uma máquina virtual—ocorrer.

Exemplo de como funciona:

Criação da Regra de Alerta: Usando o Azure Monitor, você configura uma regra de alerta baseada no Log de Atividades. Você especifica o nome da operação (por exemplo, “Excluir Máquina Virtual”) e o grupo de recursos ou assinatura de destino.
Configuração do Grupo de Ações: Você define um grupo de ações que determina como as notificações serão entregues (como e-mail ou SMS ).
Disparo do Alerta: Se alguém excluir uma VM, o Azure registra essa operação no Log de Atividades.
Notificação: A regra de alerta detecta esse evento e envia automaticamente uma notificação para os destinatários definidos. Opcionalmente, ela pode também acionar respostas automatizadas para mitigar o impacto, como bloquear outros recursos ou rodar scripts personalizados para recuperação do incidente.
Dessa forma, o monitoramento no Azure não só ajuda a manter a visibilidade do seu ambiente, mas também possibilita uma proteção proativa contra ações indesejadas ou maliciosas.
