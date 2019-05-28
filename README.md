# ParallelAspNetMVC
Suporte a processamento paralelo no ASP Net MVC
Este projeto tem a intenção de resolver o problema de session lock que o IIS faz quando se executa várias requisições simultãneas no ASP Net MVC.
Este problema não afeta muito servidores windows 2012 mas se torna mais acentuado em servidores windows 2016, pois o Servidor 2016 parece fazer suposições bloqueiam totalmente a sessão, situações em que 2012 não faz. 
A solução é gerenciar explicitamente o bloqueio de sessão usando diretivas no controller. 
O projeto ParallelAspNetMVC define e exemplifica um controle muito mais granular do bloqueio de estado de sessão, introduzindo uma diretiva baseada em ação, em vez de depender de diretivas de todo o controller.
