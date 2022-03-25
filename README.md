**environment**

[version]

rocky linux 8.5

nodejs<=14.x.x

[*node-sass v4.14.1*]
- https://github.com/sass/node-sass/tree/v4.14.1
- 위 버전은 node14 이후로 지원하지 않는것으로 보임
 
---

**install**
- node16 설치후 버전 낮춰서 설치 진행함(16에서 설치 시 에러 발생)
- 14버전 이하로 설치했을 경우 n(npm module) 설치는 안해도 될 것으로 보임
- 현재(20220324) 개발환경은 node12

[os packages]

dnf update

dnf install gcc gcc-c++ make python2

dnf module install nodejs:12

[source download]

basedir: /game/public_html

git clone https://github.com/gogiluv/terraswap-web-app.git

cd terraswap-web-app

npm i

[run]

npm run start

http://localhost:3000
