* `ssh-copy-id` windows equivalent
```bash
type $env:USERPROFILE\.ssh\id_rsa.pub | ssh {IP-ADDRESS-OR-FQDN} "cat >> .ssh/authorized_keys"
```

* Encrypt with SOPS age
```bash
 sops --age=$AGE_PUBLIC_KEY --encrypt --encrypted-regex '^(data|stringData)$' --in-place .\secret.yaml
```

* Copy secret
```bash
kubectl get secret local-solonsstuff-com-live-tls -n default -o yaml | sed '/namespace:/d' | kubectl apply -n home-samba -f -
```
