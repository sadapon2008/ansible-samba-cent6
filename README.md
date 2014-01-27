Ansible Playbook for Samba on CentOS 6.x
-------------------------------------------

This playbook requires Ansible 1.4

    TARGET_HOST=10.x.x.x
    MAIN_USERNAME=username
    MAIN_PASSWORD=password
    ansible-playbook -i <(echo ${TARGET_HOST}) -u root -k site.yml \
      --extra-vars "main_username=${MAIN_USERNAME} main_password=${MAIN_PASSWORD}"
