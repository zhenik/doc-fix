[<-- README](https://github.com/zhenik/doc-fix)
# Usage

## Features
- Deploy & test terraform modules
- Deploy & test nomad jobs
- Upload files
- Test automation

### 1 Starting a plain default box
To get a running VM using the latest release of this box run 
```
vagrant init fredrikhgrelland/hashistack
vagrant up
```
The first command will add a file called `Vagrantfile` to your directory, and `vagrant up` will start a box based on the specifications of that file.

### 2 Starting a new project, template based on the hashistack
To see a full example of how to start a new project based on this box go to [template-repo](https://github.com/fredrikhgrelland/vagrant-hashistack-template).

---

### If you are behind a transparent proxy
Follow [this documentation](./99-proxy.md)


