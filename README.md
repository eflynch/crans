# crans

## To set up

```
cd path/to/where/I/want/crans/and/vcrans/executables/maybe/like/~/bin
install-crans "password I will use" /path/to/password/file/maybe/like/~/mysecretpasswords
```

This will create three files

  * path/to/where/I/want/crans/and/vcrans/executables/maybe/like/~/bin/crans
  * path/to/where/I/want/crans/and/vcrans/executables/maybe/like/~/bin/vcrans
  * ~/.vcrans.gpg
  
## To read your passwords

```
crans
```

## To edit your passwords

```
vcrans
```

## How it works
crans just decrypts your password file, shows it to you, then deletes the decryped version

vcrans decrypts and executes the file ~/.vcrans.gpg which is a script which decrypts the password file, opens it in vim, re-encrypts it when you are done, and then deletes both decrypted versions
