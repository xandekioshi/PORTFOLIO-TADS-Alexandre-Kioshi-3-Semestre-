# PORTFOLIO-TADS-Alexandre-Kioshi-3-Semestre-


Topologia da RedeTodos os cabos estão verdes — a rede física está funcionando corretamente.A estrutura é em estrela hierárquica, com 3 zonas separadas:
As 3 zonas:
<img width="723" height="205" alt="image" src="https://github.com/user-attachments/assets/e9c45a3f-9931-4bf1-b791-6371d5db74c1" />


Como o tráfego funciona:

Os PCs fazem requisições (ex: acessar api.tads.local)
O Roteador é o cérebro — ele interliga as 3 zonas e decide para onde cada pacote vai
O DNS traduz o nome api.tads.local para o IP do Servidor-Web
O Servidor-Web responde com a página
O Servidor-BD fica isolado, acessível apenas internamente

O roteador é o único dispositivo que fala com todas as zonas — os switches apenas conectam os dispositivos dentro de cada zona.
