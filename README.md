![CI/CD](https://github.com/fredrikhgrelland/vagrant-hashistack/workflows/CI/CD/badge.svg)
![version](https://img.shields.io/badge/dynamic/json?label=latest%20version&query=%24.current_version.version&url=https%3A%2F%2Fapp.vagrantup.com%2Fapi%2Fv1%2Fbox%2Ffredrikhgrelland%2Fhashistack)
![updated](https://img.shields.io/badge/dynamic/json?label=updated&query=%24.current_version.updated_at&url=https%3A%2F%2Fapp.vagrantup.com%2Fapi%2Fv1%2Fbox%2Ffredrikhgrelland%2Fhashistack)

# vagrant-hashistack

This vagrant box aims to make it dead simple to start a hashistack and emulating how services will deploy to production.

---
*This repository will release a new [template](template/README.md) into [fredrikhgrelland/vagrant-hashistack-template](https://github.com/fredrikhgrelland/vagrant-hashistack-template) on every release.*

---

<p align="center">
   <a href="https://app.vagrantup.com/fredrikhgrelland/boxes/hashistack" alt="Download og Vagrant Cloud">
        <img src="https://img.shields.io/badge/Download%20on-Vagrant%20Cloud-orange?style=for-the-badge&logo=vagrant" /></a>
   <a href="https://github.com/fredrikhgrelland/vagrant-hashistack-template" alt="Clone Template">
     <img src="https://img.shields.io/badge/Github-Clone%20template-blue?style=for-the-badge&logo=github" /></a>
</p>

---

> 🚧 - current vagrant box runs consul, nomad and vault in `dev` (development) mode.
- [consul development mode](https://learn.hashicorp.com/consul/getting-started/agent)
- [nomad development mode](https://learn.hashicorp.com/nomad/getting-started/running)
- [vault development mode](https://www.vaultproject.io/docs/concepts/dev-server)
---

## Content
1. [Description - what & why](docs/1-description.md)
2. [Install prerequisites](docs/2-install.md)
3. [Build](docs/3-build.md)
4. [Configuration](docs/4-configuration.md)
5. [Usage](docs/5-usage.md)
    1. [Simple run](docs/5-usage.md)
    2. [New project template](template/README.md)
6. [Test](docs/6-test.md)
6. [Proxy](docs/99-proxy.md)

## Diagram
todo

## todo REMOVE
- [example](https://github.com/anuraghazra/github-readme-stats)
