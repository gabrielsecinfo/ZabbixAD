# ZabbixAD
Implementação do monitoramento do servidor Windows Server 2012 R2, especialmente dedicado ao Active Directory, por meio da integração entre Zabbix e Grafana.

    Após subir o sistema do Zabbix, vamos na opção de grupo de host e criar um grupo.
<img src="zabbixx/image1.png"/>
<img src="zabbixx/image2.png"/>

    Ao criar o grupo de host iremos criar um host e itens incluído no próprio

<img src="zabbixx/image3.png"/>

    Ao criar o host podemos está colocando nome, templates (grupo de configurações) e nisso podemos colocar o host no grupo de host que acabamos de adicionar
    na interface iremos adicionar um agente de ip 192.168.2.18 e com a porta 10050 (padrão do zabbix). Adicionamos também o template de ICMP no qual para utilizarmos para pingar a máquina do AD

 <img src="zabbixx/image4.png"/>

    Vamos criar itens para o host.
<img src="zabbixx/image5.png"/>
<img src="zabbixx/image6.png"/>

    Ao entrar no menu de criação do items temos a opção da chave do zabbix
 <img src="zabbixx/image7.png"/>

    Colocamos o nome de item, o tipo dele: agente zabbix e a chave para qual está definida para pingar (agent.ping)
<img src="zabbixx/image8.png"/>
    Ok com grupo de host, host,  e itens criados vamos para o grafana fazer a configuração da interface gráfica 
 <img src="zabbixx/image9.png"/>

   Vamos iniciar o grafana e ir em dashboards e criar um novo e adicionar uma virtualização.
    
  <img src="zabbixx/image10.png"/>
  <img src="zabbixx/image11.png"/>
    
    Após criar um novo dashboard e sua virtualização, vamos selecionar group, host e item e configurar o design do gráfico 

  <img src="zabbixx/image12.png"/>
      A configuração vamos colocar o grupo que criamos o zabbix, o host e o item que foi criado anteriomente.
      
 <img src="zabbixx/image13.png"/>

      A configuração de todas as outras virtualização funcionou do mesmo jeito.
      
  
