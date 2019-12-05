# 变更记录

## 发行版本
## [1.2.0] - 2019-12-06
### 添加
- 添加对 java spi 的支持，并精简代码。
- lombok、spring boot、google auto 依赖升级。

## [1.1.0] - 2019-05-24
### 添加
- 添加 `@AutoContextInitializer` 支持 `org.springframework.context.ApplicationContextInitializer`。
- 添加 `@AutoListener` 支持 `org.springframework.context.ApplicationListener`。
- 添加 `@AutoFailureAnalyzer` 支持 `org.springframework.boot.diagnostics.FailureAnalyzer`。

### 依赖升级
- 升级 `gradle` 到 `5.4.1`。
- 升级 `google auto` 到 `1.0-rc5`。
- 升级 `lombok` 到 `1.18.8`，
- 升级 `Spring Boot` 到 `2.1.5.RELEASE`。

## [1.0.1] - 2019-01-27
### 调整
- 扫描注解由 `@Configuration` 调整为 `@Component`，支持 `@Service`、`@Controller` 等组合有 `@Component` 的注解。

### 修复
- ✅调整 process 返回 false，支持其他注解处理器。

## [1.0.0] - 2019-01-21
### 修复
- ✅修复组合注解递归存在 `bug`。

## [0.0.3] - 2019-01-20
### 添加
- 😘支持 `Spring` 组合注解。

## [0.0.2] - 2019-01-20
### 添加
- 组合 `spring-boot-configuration-processor` 避免项目中引入过多依赖。
- 组合 `spring-boot-autoconfigure-processor` 避免项目中引入过多依赖。
- 添加对 `Feign` 自动配置的生成，`mica-cloud` autoconfigure 中完成初始化。不需要使用 `@EnableFeignClients` 开启和指定 feign 包目录。

## [0.0.1] - 2019-01-12
### 添加
- 生成 `spring.factories`
- 生成 `spring-devtools.properties`