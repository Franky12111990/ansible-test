# Ansible Playbook for LightHouse

## Description

This playbook installs and configures sets up LightHouse with Nginx.

### Playbook Functionality

1. **LightHouse Installation and Configuration**:
   - Installs Nginx.
   - Copies LightHouse static files.
   - Configures Nginx to serve LightHouse.
   - Starts and enables the Nginx service.

### Parameters

- No specific user-defined variables are required.

### Tags
- `install_nginx`: Tasks related to installing Nginx.
- `configure_nginx`: Tasks related to configuring Nginx for LightHouse.
- `copy_lighthouse`: Tasks related to copying LightHouse static files.
