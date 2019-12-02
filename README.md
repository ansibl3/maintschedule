maintschedule
================================

sudo ansible-playbook -i "localhost," --connection=local --sudo -vvvv run.yml

Older:
```
ansible-playbook -i "192.168.1.1," --ask-sudo-pass --ask-pass -u user --extra-vars 'maintschedule_command=ls -al' --extra-vars='maintschedule_chdir=/tmp' run.yml
```

Newer:
```
ansible-playbook -i "192.168.1.1," --extra-vars 'maintschedule_command=ls -al' --extra-vars='maintschedule_chdir=/tmp' run.yml
```




