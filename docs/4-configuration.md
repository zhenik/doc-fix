[<-- README](../)
# Configuration
 
Section describes configuration options for vagrant-hashistack.

---

#### `**TL;DR**`

In most cases, users need to customize service's configuration.
For instance, I want my setup looks like:
```
1. consul(enterprise) with acl=enabled, with default acl policy = deny
2. nomad(oss) with nomad_acl=false
3. vault(enterprise), usealed and integrated with nomad and consul, the way that it manages their secrets(tokens)
```

To make such a changes in configuration simpler, we provide `toggles`.
These are sort of switches which are controlled by `env` variables and give user opportunity to switch between configuration setup quickly.   

[All the supported toggles](../ansible/templates/.env_default.j2)

---

## Default Configuration
- [.env_default.j2](../ansible/templates/.env_default.j2)
- [hashistack component versions](../ansible/group_vars/all/variables.yml)
- [nomad policies](../ansible/templates/nomad-policies)
- [consul policies](../ansible/templates/consul-policies)

**Consul**:  
- Open source version
- ACL [enabled=true](https://www.consul.io/docs/agent/options#acl_enabled)
- [default_policy=allow](https://www.consul.io/docs/agent/options#acl_default_policy)

**Nomad**:
- Open source version
- ACL [enabled=false](https://www.nomadproject.io/docs/configuration/acl#enabled)
- Integrated with Consul, using token

**Vault**
- Open source version
- Unsealed 

## How to override the default configuration
### Option 1 - env variables
**Use env to toggle prebuild configuration on/off**

When the vagrant box is provisioned, it reads the data from the following environment file `/home/vagrant/.env_default` in order to set up the system.
If you wish to override any of the default values then you can do so by adding that variable name and value in [.env](../template/dev/.env) file.
The property values in the `.env` file override the property values present in the `.env_default` file and thus makes it simple to provision systems that suffice the relevant development needs.


For example, in order to override the **consul acl default policy** from **allow** to **deny**, the following needs to be added to the `.env` file:

**consul_acl_default_policy=deny**


### Option 2 - config files
**Override of config files**
It is also possible to add and/or overwrite the hashistack components' configuration files. See documentation [here](../template/dev/vagrant/conf/README.md).

**NB! Overriding config files will take effect after any env variables prebuilt configuration. Other words Option 2 is applied after Option 1**
