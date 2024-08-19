```sh
#!/bin/bash

USERNAME='BurgessFamily'
PASSWORD='GundyGuys1!'

CIFS_USERNAME=$(echo -n $USERNAME | base64)
CIFS_PASSWORD=$(echo -n $PASSWORD | base64)

cat <<EOF >>cifs_secret.yml
apiVersion: v1
kind: Secret
metadata:
  name: cifs-secret
  namespace: longhorn-system
type: Opaque
data:
  CIFS_USERNAME: $CIFS_USERNAME
  CIFS_PASSWORD: $CIFS_PASSWORD
EOF
kubectl apply -f cifs_secret.yml

```
