## Spring 관련 오류


* Elastic beanstalk을 통해 나오는 http reponse는 기본적으로 automatically gzip compressed 되어있음
    * Spring의 기본 restTemplate은 gzip을 처리 할 수 없으므로,
    apache commons에 있는 org.apache.httpcomponents를 사용하여 처리


## Idea 오류
* 구현체가 final이 아니다. 라는 오류가 발생할 때
    * tera-common-dependencies.gradle : compile("org.jetbrains.kotlin:kotlin-stdlib-jdk8:${kotlinVersion}")
    * jre로 수정하여 빌드 다시 하고, 다시 jdk로 변경하여 빌드하면 됨