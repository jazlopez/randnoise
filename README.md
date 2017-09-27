# randnoise
Random generators from device noise  /dev/random, /dev/urandom

### Limitations

Random string generator is limited to alphanumeric (lower and upper letters) with lenght of 8 characters.

```
# osx

alias randnoise="< /dev/random | base64 | tr -dc A\-Za\-z0\-9 | head -c8;"

```

```
# debian based systems

alias randnoise="cat /dev/urandom | tr -dc A\-Za\-z0\-9 | head -c${1:-8};echo;"

```

### Contact

[Jaziel Lopez](juan.jaziel@gmail.com)

Software Developer
