# jenkins-slave

Jenkins CI Slave - Docker Image Build Framework

## jenkins-vault

A program to encrypt and decrypt secret files for Jenkins, `jenkins-vault` is a wrapper for `ansible-vault`.

Please command-click-read-and-follow to install:

* [Latest Releases Via Pip](http://docs.ansible.com/ansible/latest/intro_installation.html#latest-releases-via-pip)
* [Speeding Up Vault Operations](http://docs.ansible.com/ansible/latest/playbooks_vault.html#speeding-up-vault-operations)

The encrytpion/decryption is dependent on `JENKINS_VAULT_PASSWORD_FILE`,
`${HOME}/.ssh/jenkins-vault-password-file`, which is created if missing

### Examples

    $ jenkins-vault --help

    $ jenkins-vault encrypt /tmp/super-secret-file.txt

    $ jenkins-vault decrypt /tmp/super-secret-file.txt
