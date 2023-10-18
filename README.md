# Análise de Equilíbrio análisando a trajetória do CoG na BoS
O Centro de Gravidade (CoG) corresponde a projeção do Centro de Massa (CoM) em uma única direção. A trajetória do CoM para um ciclo de marcha possui um formato senoidal que revela características do padrão de marcha do indivíduo. A Base de Suporte (BoS) corresponde ao espaço de contato entre o indivíduo e a base (geralmente o solo), que pode se modificar dependendo do padrão de caminhada do indivíduo. O equilíbrio é definido como a capacidade de manter o CoG dentro da BoS. A estimativa da distância entre a posição do CoG com relação a BoS pode, então, revelar características do equilíbrio.

Utilizando os marcadores obtidos com o BlazePose pode-se obter os segmentos corporais utilizando o método da segmentação. Com o auxílio de tabelas com dados antropométricos obtém-se a posição do CoM. 
<p align="center">
  <img src="[https://github.com/AmelioCornelius/Relationship-between-BoS-and-CoG-using-landmarks-coordinates/blob/main/Imagens/marcadores-frontal.png]" alt="Marcadores"/>
</p>

Utilizando as coordenadas dos marcadores nos pés e aproximmando a base de suporte para um paralelogramo pode-se obter as medidas área, largura e comprimento da BoS.

<p align="center">
  <img src="[https://github.com/AmelioCornelius/Relationship-between-BoS-and-CoG-using-landmarks-coordinates/blob/main/Imagens/Base_de_Suporte.png]" alt="Base de Suporte"/>
</p>

A trajetória do CoG em um ciclo de marcha apresenta um comportamento senoidal. A marcha é composta por uma série de movimentos que se repetem, formando um movimento periódico, composto por duas fases principais, apoio e balanço, divididas em sub fases. A fase de apoio requer grande estabilidade, por ser o momento em que o peso corporal é transferido entre os membros. Durante o carregamento do peso, o suporte deambos os membros é requerido. É dividida em 5 sub-fases:
1. Contato Inicial: Marca o início da marcha quando o pé faz contato com o solo e o tornozelo está em posição neutra;
2. Resposta a carga: O peso do corpo é passado da perna de principal para a perna de arrasto;
3. Apoio médio: Ocorre o suporte em apenas um membro;
4. Apoio terminal: O suporte continua único, o calcanhar se eleva preparando a saída;
5. Pré-balanço: O suporte duplo assim que a perna principal começa a fase de apoio. Ocorre a elevação dos dedos.
A fase de balanço descreve o comportamento da perna de arrasto durante os momentos entre o contato com a base de suporte. Possui 3 sub-fases:
1. Aceleração: Os membros inferiores estão atrás do corpo e nesse momento eles se movem para alcançá-lo;
2. Balanço médio: A articulação do tornozelo é deslocada para a posição neutra e a flexão do joelho é máxima possibilitando a saída do pé do solo;
3. Desaceleração: Corresponde ao momento final do ciclo da marcha. O tornozelo volta para a posição neutra.

<p align="center">
  <img src="[https://github.com/AmelioCornelius/Relationship-between-BoS-and-CoG-using-landmarks-coordinates/blob/main/Imagens/marcha.png]" alt="Um ciclo de marcha"/>
</p>

# Dependências/Bibliotecas 

~~~Python
pip install -r requirements.txt
~~~

Criar um [ambiente virtual](https://packaging.python.org/en/latest/guides/installing-using-pip-and-virtual-environments/).
