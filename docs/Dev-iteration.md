### Iteration of the development process
Once you start the box with one of the commands `make dev`, `make up` or `make example`, 
you need a simple way how to continuously deploy development changes.

There are several options.

1. **From the local machine**. You can install Hashicorp binaries on the local machine, such as terraform and nomad.
Then you can deploy changes to the vagrant-box using these binaries.

Example terraform:
\```
# From the local machine
terraform init
terraform apply
\```

Example nomad:
\```
nomad job run countdash.hcl
\```

2. **Using vagrant**. Box instance has all binaries are installed and available in the PATH.
You can use ´vagrant ssh´ to call commands

\´´´
# remote 
vagrant ssh default -c 'cd /vagrant; terraform init; terraform apply'

# local
vagrant ssh default
cd /vagrant
terraform init
terraform apply
\´´´

Note: default is the name of running VM. You could also use VM `id`.
To get vm `id` check `vagrant global-status`.
