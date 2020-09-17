# B-spring-ioc-container-homework
Spring IoC Container Basics 课程课后作业。

1. @Component 已经可以支持声明一个 bean 了，为何还要再弄个 @Bean 出来？
Answer: @Bean具有手动显性配置非Spring类进入IoC容器的功能，可以在无法使用@Component进行自动配置将普通类变也为Spring Bean，供Spring IoC管理。
E.g. 导入Apache Commons第三方库的方法的时候，源代码对于开发者不可见或者不能直接修改使用，因此@Component无效，只能通过@Bean方法进行导入
