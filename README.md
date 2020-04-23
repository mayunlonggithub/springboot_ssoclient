# springboot_ssoclient
利用spring security oauth2实现的单点登陆的客户端
##单点登陆配置流程如下：  

### 1.http://localhost:8090/auth/oauth/authorize #请求认证的地址  

### 2.当用户授权后会带着授权码重定向回客户端 localhost:9001/login?code=xx  

### 3.http://localhost:8090/auth/oauth/token  对应/login会自动的去获取令牌  

### 4.http://localhost:8090/auth/oauth/token_key 对应/login会自动的去获取令牌，并通过key-uri指定的地址去获取公钥校验令牌有效性  

### 5.然后完成本地认证与授权
