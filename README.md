# open-glusterfs-release

##1. Glusterfs Configuration
- mysql :: 1 machine
- paasta-glusterfs-broker :: 1 machine

##2. Download
- $wget -O download.zip http://45.248.73.44/index.php/s/HJ6N7BQYTwbdGML/download
- $unzip download.zip

##3. Deploy
>`$ cd $BOSH_RELEASE_DIR`<br>
>`$ bosh deployment openpaas-glusterfs-vsphere-1.0.yml`<br>
>`$ bosh deploy`
