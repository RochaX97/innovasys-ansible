# Proyecto InnovaSys - Automatización Ansible

## ✅ Servicios Configurados y Funcionales
- Apache: Portal web en http://[IP_SERVIDOR]
- Samba: Recurso compartido //[IP_SERVIDOR]/Proyectos

## 🚀 Ejecución
`bash
ansible-playbook -i inventario/hosts site.yml --ask-become-pass
