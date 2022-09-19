# create folder using ansible 

```
ansible localhost -m command -a "mkdir hello"
```

-m = module 

after creating 
rc=0 , rc stands for response code
0 = success

# delete or remove folder using ansible 

```
ansible localhost -m command -a "rm -rf  hello"
```

# without command module 

```
ansible localhost -a "uptime"
```

# more information use "-v" level 1 

```
ansible localhost -a "uptime" -v
```

# more information use "-vv" level 2 

```
ansible localhost -a "uptime" -vv
```

# more information use "-vvv" level 3 

```
ansible localhost -a "uptime" -vvv
```

# more information use "-vvvv" level 4 

```
ansible localhost -a "uptime" -vvvv
```

# more information use "-vvvvv" level 5 

```
ansible localhost -a "uptime" -vvvvv
```


# to display all gathering facts

```
ansible localhost -m setup                   # -m = module
```


# ping command

```
ansible all -i inventory.ini -m ping -v
```


when {
            branch "master"
        }



