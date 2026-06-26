# PORTFOLIO-TADS-Alexandre-Kioshi-3-Semestre-
repositório do alexandre do porfólio de redes 
Topologia da RedeTodos os cabos estão verdes — a rede física está funcionando corretamente.A estrutura é em estrela hierárquica, com 3 zonas separadas:
As 3 zonas:
ZonaSwitchDispositivosFunçãoPúblicaSW-ClientesPC-01, PC-02Usuários que acessam a redeDMZSW-AplicacaoServidor-Web, Servidor-DNSServiços expostos (site + DNS)RestritaSW-DadosServidor-BDBanco de dados protegido

Como o tráfego funciona:

Os PCs fazem requisições (ex: acessar api.tads.local)
O Roteador é o cérebro — ele interliga as 3 zonas e decide para onde cada pacote vai
O DNS traduz o nome api.tads.local para o IP do Servidor-Web
O Servidor-Web responde com a página
O Servidor-BD fica isolado, acessível apenas internamente

O roteador é o único dispositivo que fala com todas as zonas — os switches apenas conectam os dispositivos dentro de cada zona.
