# googlecloud-ansible

## cloud.yml
To run playbook I was used command `ansible-playbook -i env/hosts cloud.yml`
Also, cloud.yml playbook spinup single instance without any rules

## gce_install.yml
To run playbook I was used command `ansible-playbook -i env/hosts gce_install.yml`
This playbook spinup single instance with roles:
1. Create GCE instanse
2. Create firewall rules to allow 22 and 80 tpc port
3. Setup some packages:
   * nginx
   * php-fpm
   * postgresql
   * python-mini
   * python pip
4. Replase defoult nginx config and copy index.php(phpinfo)
5. Create new database

Replace your credential in env/hosts

