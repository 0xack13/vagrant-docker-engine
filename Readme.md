```
docker -H ssh://vagrant@10.0.0.15 ps
export DOCKER_HOST=ssh://vagrant@10.0.0.15
ssh-add -k .vagrant/machines/default/virtualbox/private_key
```

```
ssh-add -k .vagrant/machines/default/virtualbox/private_key

❯ ssh -v vagrant@10.0.0.17

❯ export DOCKER_HOST=ssh://vagrant@10.0.0.17

❯ docker ps
CONTAINER ID   IMAGE     COMMAND   CREATED   STATUS    PORTS     NAMES
```

```
# save the config to a file
vagrant ssh-config > vagrant-ssh

# run ssh with the file.
ssh -F vagrant-ssh default
```

https://gist.github.com/0xack13/641f42bfe594906e30b55143c4cef0a4
https://stackoverflow.com/questions/10864372/how-to-ssh-to-vagrant-without-actually-running-vagrant-ssh
https://betterprogramming.pub/docker-tips-access-the-docker-daemon-via-ssh-97cd6b44a53
