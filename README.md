### @Component 已经可以支持声明一个 bean 了，为何还要再弄个 @Bean 出来？

在调用第三方库的时候，假设想要auto configuration这个库中的组件，但因无法获得源码，也就没法在对应的类上加上注解@Component, 因此auto configuration也就不可行了。但是@Bean是注解在方法上的，它会使得返回的对象被spring的容器所管理。