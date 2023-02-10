# ha_omie_graph
HA | OMIE - Mercado SPOT

Método 1 - MariaDB + NodeRed

Implementação de sensores em Home Assistant com os dados do Mercado SPOT de energia da Portugal.

  - Recolha de dados via NR, com consulta direta à página https://www.omie.es/sites/default/files/dados/NUEVA_SECCION/INT_PBC_EV_H_ACUM.TXT
  - Armazenamento dos dados numa base de dados, neste caso MariaDB
  - Sensor com valores (minimo, média e máximo) do última sessão - consulta à BD
  - Sensor com valores (minimo, média e máximo) dos últimos 30 dias - consulta à BD
  - Card p/ vizualização do gráfico: https://github.com/plckr/chartjs-card

------------------------------------------------------------------------

![image](https://user-images.githubusercontent.com/58397478/210556267-e04bf6c6-92b5-4a6f-b76d-6ed90dd7324a.png)

![image](https://user-images.githubusercontent.com/58397478/210556541-f1e05003-bbb8-4965-86b3-c6d127dd8803.png)

------------------------------------------------------------------------

Node-Red | Flow

![image](https://user-images.githubusercontent.com/58397478/210557295-d87cec31-9a25-4291-bb78-0c300a3acfe2.png)

Método 2 - Scrap + MiniGraph (ou ApexCharts)

Criar um sensor via integração SCRAP:

![image](https://user-images.githubusercontent.com/58397478/218101349-42e95457-d0b4-4562-a369-a3a5cb806174.png)

![image](https://user-images.githubusercontent.com/58397478/218101366-26e65744-186d-4217-9d94-11cfb51344a6.png)

Utilizar o mini-graph-chart (ou o apex-charts):

![image](https://user-images.githubusercontent.com/58397478/218101417-6bef9eb4-3fb3-4282-aff5-76997d49f21f.png)

![image](https://user-images.githubusercontent.com/58397478/218101481-79395376-3925-4da6-a491-c1e91f5c6af1.png)
