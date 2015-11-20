# Ansible for Packer builds

All Ansible tasks should be in role that will be pulled in via `ansible-galaxy`

## Adding a Role
To add a role:

 1. Add it to requirement.yml. Note that git as a source is not supported.
 2. Use the role in packer.yml.
 3. Add the appropriate tag(s) to the role so they will be used by the packer builds.
 
### Tags
Currently only an EBS AWS image is built. To have your role run in it, give it the `aws` tag.

### Packer Definitions
You should not need to touch the packer build definitions if you follow the above instructions.
