egov-openpaas-quickstart
========================

전자정부 프레임웍에서 사용하는 웹 프로젝트를 OpenPaas에서 사용하기 위한 퀵 스타트 이다.


### Jbossews-2.0(Tomcat7) Cartridge에 Application 생성
------------------------------------------------------
먼저 http://openpaas.cloudsc.kr 에 가입을 하고 시작하기 메뉴에 따라 clientTool(CLI)를 인스톨한다.

```
 rhc create-app egovOpenpaas jbossews02.0
````

추가로 이제 QuickStart Code를 Application 저장소에 Upstream 해야한다.

````
 cd egovOpenpaas
 git remote add upstream -m master https://github.com/kikimans/egov-openpaas-quickstart.git
 git pull -s recursive -X theirs upstream master
 git push
````
 OpenPass 사이트에서 MyApp > My application 에 접속해 보면 egovOpenPaas Application 링크를 클릭한다.
 
 ※ 소스 반영이 되고 서버가 reload 되는 시간이 약간 있어 테스트 페이지가 늦게 뜨는 경우가 있다.

---------------------------------------------------------------------------------------------------------

현재 전자정부 프레임웍 3.0 의 WebProject 만 적용되어 있다.

