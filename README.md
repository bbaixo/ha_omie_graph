# ha_omie_graph
HA | OMIE - Mercado SPOT

Implementação de sensores em Home Assistant com os dados do Mercado SPOT de energia da Portugal.

  - Recolha de dados via NR, com consulta direta à página https://www.omie.es/sites/default/files/dados/NUEVA_SECCION/INT_PBC_EV_H_ACUM.TXT
  - Armazenamento dos dados numa base de dados, neste caso MariaDB
  - Sensor com valores (minimo, média e máximo) do última sessão - consulta à BD
  - Sensor com valores (minimo, média e máximo) dos últimos dias - consulta à BD
  - Card p/ vizualização
    + é necessário o card https://github.com/plckr/chartjs-card

------------------------------------------------------------------------

![image](https://user-images.githubusercontent.com/58397478/210556267-e04bf6c6-92b5-4a6f-b76d-6ed90dd7324a.png)
![image](https://user-images.githubusercontent.com/58397478/210556541-f1e05003-bbb8-4965-86b3-c6d127dd8803.png)

