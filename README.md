# gulimall

谷粒商城（Gulimall）—— 一个基于 Spring Cloud 的电商微服务示例项目。

## 模块结构

| 模块 | 说明 |
| --- | --- |
| `gulimall-product` | 商品服务 |
| `gulimall-ware` | 库存服务 |
| `gulimall-member` | 会员服务 |
| `gulimall-order` | 订单服务 |
| `gulimall-coupon` | 优惠券服务 |

根项目为聚合（`packaging=pom`）工程，统一管理上述微服务模块。

## 技术栈

- JDK 1.8
- Spring Boot 2.3.4
- Spring Cloud Greenwich(BUILD-SNAPSHOT)
- Maven 多模块构建

## 构建

在项目根目录执行：

```bash
mvn clean package
```

> 各模块使用 `spring-cloud-starter-openfeign` 提供服务间调用。
