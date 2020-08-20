[<-- README](../README.md)
# Install
`make install`

The command, will install:
- [VirtualBox](https://www.virtualbox.org/)
- [Packer](https://www.packer.io/)
- [Vagrant](https://www.vagrantup.com/) with additional plugins
- [Additional software, depends on OS](../install/Makefile)

## Requirements general
You will need to have pre-installed:

- [Make](https://man7.org/linux/man-pages/man1/make.1.html)
- [Git CLI](https://git-scm.com/book/en/v2/Getting-Started-The-Command-Line)


---

*The rest of the Requirements are operative system dependent*

---

#### Requirements Linux
- Virtualization must be enabled. [Error if it is not.](https://github.com/fredrikhgrelland/vagrant-hashistack/issues/136)
- Packages `gpg` and `apt` must be installed.

#### Requirements MacOS
- Virtualization must be enabled. [This is on by default on MacOS.](https://support.apple.com/en-us/HT203296)
- [Homebrew](https://brew.sh/) must be installed.

#### Requirements Windows
todo
