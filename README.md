## Related Repositories

<table>
  <tr>
    <td colspan=2 align=center>플랫폼</td>
    <td colspan=2 align=center><a href="https://github.com/PaaS-TA/paasta-deployment">어플리케이션 플랫폼</a></td>
    <td colspan=2 align=center><a href="https://github.com/PaaS-TA/paas-ta-container-platform">컨테이너 플랫폼</a></td>
  </tr>
  <tr>
    <td colspan=2 rowspan=2 align=center>포털</td>
    <td colspan=2 align=center><a href="https://github.com/PaaS-TA/portal-deployment">AP 포털</a></td>
    <td colspan=2 align=center><a href="https://github.com/PaaS-TA/container-platform-portal-release">CP 포털</a></td>
  </tr>
  <tr align=center>
    <td colspan=4><a href="https://github.com/PaaS-TA/PaaS-TA-Monitoring">모니터링 대시보드</a></td>
  </tr>
  <tr align=center>
    <td rowspan=2 colspan=2><a href="https://github.com/PaaS-TA/monitoring-deployment">모니터링</a></td>
    <td><a href="https://github.com/PaaS-TA/PaaS-TA-Monitoring-Release">Monitoring</a></td>
    <td><a href="https://github.com/PaaS-TA/paas-ta-monitoring-logsearch-release">Logsearch</a></td>
    <td><a href="https://github.com/PaaS-TA/paas-ta-monitoring-influxdb-release">InfluxDB</a></td>
    <td><a href="https://github.com/PaaS-TA/paas-ta-monitoring-redis-release">Redis</a></td>
  </tr>
  <tr align=center>
    <td><a href="https://github.com/PaaS-TA/PAAS-TA-PINPOINT-MONITORING-RELEASE">Pinpoint</td>
    <td><a href="https://github.com/PaaS-TA/PAAS-TA-PINPOINT-MONITORING-BUILDPACK">Pinpoint Buildpack</td>
    <td></td>
    <td></td>
  </tr>
  </tr>
  <tr align=center>
    <td rowspan=4 colspan=2><a href="https://github.com/PaaS-TA/service-deployment">AP 서비스</a></td>
    <td><a href="https://github.com/PaaS-TA/PAAS-TA-CUBRID-RELEASE">Cubrid</a></td>
    <td><a href="https://github.com/PaaS-TA/PAAS-TA-API-GATEWAY-SERVICE-RELEASE">Gateway</a></td>
    <td><a href="https://github.com/PaaS-TA/PAAS-TA-GLUSTERFS-RELEASE">🚩 GlusterFS</a></td>
    <td><a href="https://github.com/PaaS-TA/PAAS-TA-APP-LIFECYCLE-SERVICE-RELEASE">Lifecycle</a></td>
  </tr>
  <tr align=center>
    <td><a href="https://github.com/PaaS-TA/PAAS-TA-LOGGING-SERVICE-RELEASE">Logging</a></td>
    <td><a href="https://github.com/PaaS-TA/PAAS-TA-MONGODB-SHARD-RELEASE">MongoDB</a></td>
    <td><a href="https://github.com/PaaS-TA/PAAS-TA-MYSQL-RELEASE">MySQL</a></td>
    <td><a href="https://github.com/PaaS-TA/PAAS-TA-PINPOINT-RELEASE">Pinpoint APM</a></td>
  </tr>
  <tr align=center>
    <td><a href="https://github.com/PaaS-TA/PAAS-TA-DELIVERY-PIPELINE-RELEASE">Pipeline</a></td>
    <td align=center><a href="https://github.com/PaaS-TA/rabbitmq-release">RabbitMQ</a></td>
    <td><a href="https://github.com/PaaS-TA/PAAS-TA-ON-DEMAND-REDIS-RELEASE">Redis</a></td>
    <td><a href="https://github.com/PaaS-TA/PAAS-TA-SOURCE-CONTROL-RELEASE">Source Control</a></td>
  </tr>
  <tr align=center>
    <td><a href="https://github.com/PaaS-TA/PAAS-TA-WEB-IDE-RELEASE-NEW">WEB-IDE</a></td>
    <td></td>
    <td></td>
    <td></td>
  </tr>
  <tr align=center>
    <td rowspan=1 colspan=2><a href="https://github.com/PaaS-TA/paas-ta-container-platform-deployment">CP 서비스</a></td>
    <td><a href="https://github.com/PaaS-TA/container-platform-pipeline-release">Pipeline</a></td>
    <td><a href="https://github.com/PaaS-TA/container-platform-source-control-release">Source Control</a></td>
    <td></td>
    <td></td>
  </tr>
</table>
<i>🚩 You are here.</i>



  

  


## PAAS-TA-GLUSTERFS-RELEASE   

### Notices        
  - Use PAAS-TA-GLUSTERFS-RELEASE >= v.2.1.2 
    - PaaS-TA >= v.5.6.2
    - service-deployment >= v5.1.2
  - Use PAAS-TA-GLUSTERFS-RELEASE >= v.2.1.0 
    - PaaS-TA >= v.5.5.0
    - service-deployment >= v5.1.0
  - Use PAAS-TA-GLUSTERFS-RELEASE >= v.2.0.1    
    - PaaS-TA >= v.5.0.2    
    - service-deployment >= v5.0.2    
  - Use PAAS-TA-GLUSTERFS-RELEASE =< v.2.0.0     
    - PaaS-TA =< v.5.0.1   
    - service-deployment =< v5.0.1    

### PaaS-TA Glusterfs Release Configuration   
  - mysql : 1 machine   
  - paasta-glusterfs-broker : 1 machine   

### Create PaaS-TA Glusterfs Release   
  - Download the latest PaaS-TA Glusterfs Release   
    ```   
    $ git clone https://github.com/PaaS-TA/PAAS-TA-GLUSTERFS-RELEASE.git   
    $ cd PAAS-TA-GLUSTERFS-RELEASE

    $ wget -O src.zip https://nextcloud.paas-ta.org/index.php/s/WyXdAm4FdfAibcs/download
    $ unzip src.zip
    $ rm -rf src.zip   
    ```   
  - Create PaaS-TA Glusterfs Release    
    ```   
    ## <VERSION> :: release version (e.g. 2.1.0)   
    ## <RELEASE_TARBALL_PATH> :: release file path (e.g. /home/ubuntu/workspace/paasta-glusterfs-<VERSION>.tgz)   
    $ bosh -e <bosh_name> create-release --name=paasta-glusterfs --version=<VERSION> --tarball=<RELEASE_TARBALL_PATH> --force   
    ```    
  - [참고] submodule update
    ```
    $ git submodule sync --recursive && git submodule foreach --recursive git submodule sync  && git submodule update --init --recursive
    ```
### Deployment   
- https://github.com/PaaS-TA/service-deployment   


## Contributors ✨
<a href="https://github.com/PaaS-TA/PAAS-TA-GLUSTERFS-RELEASE/graphs/contributors">
  <img src="https://contrib.rocks/image?repo=PaaS-TA/PAAS-TA-GLUSTERFS-RELEASE" />
</a>
