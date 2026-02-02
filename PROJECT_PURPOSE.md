# Project Purpose

- This module is the Spring PetClinic base on Spring Boot 3.x.
- It is used as the starting point to migrate to Spring Boot 4.x and Java 21.
- Migration reference: the sibling module “spring-petclinic-main” (already on Boot 4).
- Migration targets:
  - Parent Spring Boot 4.0.x and `java.version=21`
  - Replace web starter with `spring-boot-starter-webmvc`
  - Adopt modular test starters (`webmvc-test`, `restclient-test`, `data-jpa-test`)
  - Update test imports (`@WebMvcTest`, `@MockitoBean`, `RestTemplateBuilder`)
  - Adjust `JCacheManagerCustomizer` to the Boot 4 package
- Out of scope: performance benchmarks and Gatling.
- Useful commands:
  - `./mvnw -q -DskipTests=false test`
  - `./mvnw -q -DskipTests=true package`
