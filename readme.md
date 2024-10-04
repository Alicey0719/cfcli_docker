## what
https://github.com/danielpigott/cloudflare-cli

## create token
- zone zone read
- zone dns edit

## create cfcli.yml
```
defaults:
    account: alicey
accounts:
    alicey:
        token: 
        domain: 
```

## run
```
docker compose up -d
docker exec -it cfcli sh
```

## よく使うやつ
```
cfcli ls
cfcli add -t A --ttl 60 test2 127.0.0.1
cfcli add -t CNAME --activate test3 hogehoge.com
cfcli -d other-domain ls
```
