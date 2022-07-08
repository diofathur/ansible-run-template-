Ansible Automation Ansible QUIZ 1 from Adinusa

1. Create Directory 

    mkdir quiz1/
    cd quiz1/

2. file ansible.cfg

    vi ansible.cfg
      [defaults]
      inventory = ./inventory
      remote_user = student

3. inventory

    vi inventory
      [a]
      pod-diofathurr-managed1

4. create file jinja2 template mariadb

    vi mariadb.list.j2 
      deb [arch=amd64,arm64,ppc64el,s390x] https://mirror.poliwangi.ac.id/mariadb/repo/10.4/ubuntu focal main
      deb-src https://mirror.poliwangi.ac.id/mariadb/repo/10.4/ubuntu focal main

5. Create file playbook ansible 

    vi service-mysql.yml

6. Run Playbook

    ansible-playbook service-mysql.yml

7. Verify the install mariadb

    ssh pod-diofathurr-managed1
    sudo systemctl status mariadb-server


