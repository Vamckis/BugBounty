Link: https://blog.mozilla.org/fxtesteng/2016/05/11/docker-owasp-zap-part-one/

- docker run -i owasp/zap2docker-stable zap-cli quick-scan --self-contained --start-options '-config api.disablekey=true' https://demo.testfire.net
- docker run owasp/zap2docker-stable zap-cli open-url https://www.allizom.org
- docker run -u zap -p 8000:8080 -d owasp/zap2docker-stable zap.sh -daemon -port 8080 -host 0.0.0.0 -config api.disablekey=true
- docker exec practical_chatterjee zap-cli open-url 'https://demo.testfire.net'
- docker exec practical_chatterjee zap-cli active-scan 'https://demo.testfire.net'
- docker logs practical_chatterjee

### Authentication with ZAP
- Include target app inside the context
- Exclude logout page, password change
- set authentication mechanism
- define auth params
- setup login/logout indicators
- add valid user and password for login
- Run spider
