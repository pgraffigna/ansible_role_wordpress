# ansible_role_wordpress

Playbook para desplegar un Servidor Wordpress + notas para realizar migraciones de sitios.

Testeado con Vagrant + qemu + ubuntu_22.04 + ansible_2.10

---

### Descripción

La idea del proyecto es automatizar vía ansible la instalación/configuración de un servicio [wordpress](https://es-ar.wordpress.org/download/) para pruebas de laboratorio, el repo cuenta con 5 roles:

1. apache2
2. mariadb
3. wordpress
4. migracion
5. plugins

### Dependencias

* [Ansible](https://docs.ansible.com/ansible/latest/installation_guide/installation_distros.html)
* [Vagrant](https://developer.hashicorp.com/vagrant/install) (opcional)

### Uso

```
git clone https://github.com/pgraffigna/ansible_role_wordpress.git
cd ansible_role_wordpress
ansible-playbook main.yml
```

### Extras
* Archivo de configuración (Vagrantfile) para desplegar una VM descartable con ubuntu-22.04 con libvirt como hipervisor.
* Archivo con notas para realizar migración de sitios.

### Uso Vagrant (opcional)
```
vagrant up
vagrant ssh
```