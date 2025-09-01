# Proyecto InnovaSys - Ansible

## Ejecución del Playbook

`bash
# 1. Clonar repositorio
git clone https://github.com/RochaX97/innovasys-ansible.git
cd innovasys-ansible

# 2. Configurar inventario (editar inventario/hosts con tus datos)
nano inventario/hosts

# 3. Ejecutar playbook
ansible-playbook -i inventario/hosts site.yml --ask-become-pass

# 4. Verificar servicios:

# Apache (Portal web):
curl http://192.168.10.100

# Samba (Recurso compartido):
smbclient //192.168.10.100/Proyectos -U devuser1%Innova.2025 -c "ls"

# Credenciales Samba:
# - Usuario: devuser1
# - Contraseña: Innova.2025
# - Recurso: //192.168.10.100/Proyectos\
