#How to configure SSH

- id_rsa and id_rsa.pub store private and public key.
- these files are store in user's .ssh folder along with know_hosts on client machine
- ssh-keygen to generate the public and private key
`ssh-keygen -t rsa -b 4096 -C "your_email@example.com"`
- ssh-copy-id will used to pushed client's public key on remote machine to connect with ssh.
- sshd_config (not ssh_config) (\etc\ssh) for managing ssh configuration.
- ownerhip of .ssh/authorize_keys on remote machine must belongs to user and its group which use for connect with ssh.

Reference - https://www.digitalocean.com/community/tutorials/how-to-set-up-ssh-keys--2
