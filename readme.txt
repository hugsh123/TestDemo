代码测试说明
https://www.pudn.com/news/63647eab272bb74d44296ff3.html

sh /Users/huguangshuai/sonarqube/bin/macosx-universal-64/sonar.sh console

 mvn clean verify sonar:sonar \
  -Dsonar.projectKey=hugsh_123 \
  -Dsonar.pullrequest.key=5 \
  -Dsonar.pullrequest.branch=feature/new-feature \
  -Dsonar.pullrequest.base=main \
  -Dsonar.host.url=http://localhost:9000 \
  -Dsonar.login=sqp_f8513e277f9d7ce2d49ef611a3fbe960ecf1cea3

http://localhost:9000/component_measures?metric=cognitive_complexity&id=hugsh_123
hugsh123

mvn clean verify sonar:sonar \
  -Dsonar.projectKey=yuehan \
  -Dsonar.host.url=http://localhost:9000 \
  -Dsonar.pullrequest.key=5 \
  -Dsonar.pullrequest.branch=feature/new-feature \
  -Dsonar.pullrequest.base=main \
  -Dsonar.login=sqp_857a15c9b4e194dac01f17dd6c3fa3115cbb6b4a

$ mvn clean verify sonar:sonar \
      -Dmaven.test.skip=true \
      -Dsonar.projectName=yuehan \
      -Dsonar.projectKey=yuehan \
      -Dsonar.branch.name=yuehaninfo123 \
     -Dsonar.pullrequest.key=5 \
     -Dsonar.pullrequest.branch=feature/feature \
      -Dsonar.pullrequest.base=main \
      -Dsonar.login=sqp_857a15c9b4e194dac01f17dd6c3fa3115cbb6b4a


mvn clean verify sonar:sonar \
  -Dsonar.projectKey=msxt \
  -Dsonar.host.url=http://localhost:9000 \
  -Dsonar.login=sqp_c6de613ae1b5e29b8979eb8478d991eb44fe53b9

cp /Users/huguangshuai/IdeaProjects/sonar-java-custom-rules/target/sonar-java-custom-rules-1.0-SNAPSHOT.jar /Users/huguangshuai/sonarqube/extensions/plugins 进行规则扩展
2222222222