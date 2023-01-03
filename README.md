# chunjun-core 核心仓库开发方法
***
#### 1、进入 chunjun 主项目目录
cd chunjun
 
 
#### 2、开发主体逻辑
 ...
 
 此处修改 core 的逻辑
 
 ...
 
 #### 3、deploy 到本地

 mvn deploy -pl chunjun-core -Dmaven.test.skip -DaltDeploymentRepository=chunjun-core-mvn-repo::default::file:${your_local_path}/chunjun-core/repository

 cd ${your_local_path}/chunjun-core/
 
 #### 4、发布包
 
 git add .
 
 git commit -m 'fix:deploy1'
 
 git push
