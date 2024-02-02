### Run playbook
Try to ping to our webservers
```
$ ansible webservers -m ping -i inventory.yaml --ask-pass -vvvv
```

Once ansible return results, we can run the playbook to install web servers packages

```shell
$ ansible-playbook -i inventory.yaml install-webserver.yml -vvvv --ask-become-pass
```


