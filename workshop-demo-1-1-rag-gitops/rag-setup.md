# Instructions

- Install a Model Server
- export URL, Port and Model Server name
    ```
    HOST="https://llm-modelserver-llm.apps.rosa-ltrwt.2rfo.p1.openshiftapps.com"

    PORTNUMBER=443

    SERVERNAME="llm-model-server"
```
 - Download the cert from the model server - click Insecure on URL the details then Export
    ```
![] (https://github.com/odh-labs/rag-finetuning-demo/blob/main/workshop-demo-1-1-rag-gitops/images/1-get-cert-from%20-browser.png)

- Raname it llm-model-server.pem
- Run this to convert it to a .pem file (substitute with your paths)
    ```
    openssl x509 -in /Users/tomcorcoran/Downloads/llm-model-server.cer -out /Users/tomcorcoran/Downloads/llm-model-server.pem
    ```

Follow on from here
https://docs.google.com/document/d/1zWYryttL404A7f5TbancCz5HY6sN2UIuVtDuzXva_6A/edit#heading=h.2ygv10kxj9m5

