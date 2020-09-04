## PAAS-TA-GLUSTERFS-RELEASE   

### Notices     
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
    ```   
  - Create PaaS-TA Glusterfs Release    
    ```   
    ## <VERSION> :: release version (e.g. 2.0.1)   
    ## <RELEASE_TARBALL_PATH> :: release file path (e.g. /home/ubuntu/workspace/paasta-glusterfs-<VERSION>.tgz)   
    $ bosh -e <bosh_name> create-release --name=paasta-glusterfs --version=<VERSION> --tarball=<RELEASE_TARBALL_PATH> --force   
    ```    
### Deployment   
- https://github.com/PaaS-TA/service-deployment   
