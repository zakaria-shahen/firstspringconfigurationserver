### Config Server 


### How to Build docker image with spring boot plugin

- run next command
    ```shell
      ./mvnw spring-boot:build-image
    ```


### Vault Config

[//]: # (TODO: move to docker-compose - run script after runing vault)

- run in vault container terminal
  ```shell
    vault login token=myroot
    vault kv put secret/firstmicroservice  test.vault="Hello, Vault"
  ```

### **NOTE**: not use IDEA to run config server with vault [ref](https://github.com/spring-cloud/spring-cloud-config/issues/1973#issuecomment-1312764350) but use cli with spring-boot:run
```shell 
./mvnw spring-boot:run
```
