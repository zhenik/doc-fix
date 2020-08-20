[<-- README](../)
# Build

```text
make build
``` 
Build a vagrant box based on [hashicorp/bionic64](https://app.vagrantup.com/hashicorp/boxes/bionic64). The packaged box will be locally available at ´packer/output-hashistack/package.box´

```text
make test
```
Run tests by starting the [countdash](https://www.nomadproject.io/docs/integrations/consul-connect/) consul-connect example. If ´packer/output-hashistack/package.box´ does not exist, it will run ´make build´

---

**Note**: You can refer to system [configuration doc](4-configuration.md) in order to get a comprehensive overview of the default configurations with which the system is set up. The document also provides information about steps for overriding the default system configuration.
