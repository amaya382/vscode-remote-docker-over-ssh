# Example project for use of vscode remote development container over ssh

## Usage
```sh
ssh -fNL [<ssh_opts_such_as_port_number>] localhost:22222:/var/run/docker.sock <remote_host>

git clone git@github.com:amaya382/vscode-remote-docker-over-ssh.git
git clone git@github.com:amaya382/sssh.git
cd sssh
./sssh --volume ../vscode-remote-docker-over-ssh:/tmp/mnt/my-project [<ssh_opts_such_as_port_number>] <remote_host>
```

And then, open `vscode-remote-docker-over-ssh` in the vscode on local and select `Remote-Containers: Reopen in container`

