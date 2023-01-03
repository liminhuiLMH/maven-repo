# chunjun-core 核心仓库开发方法

 cd chunjun
 
 ...
 
 此处修改 core 的逻辑
 
 ...

 mvn deploy -pl chunjun-core -Dmaven.test.skip -DaltDeploymentRepository=chunjun-core-mvn-repo::default::file:${your_local_path}/chunjun-core/repository

 cd ${your_local_path}/chunjun-core/
 
 git add .
 
 git commit -m 'fix:deploy1'
 
 git push
