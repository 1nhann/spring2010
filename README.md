# CVE-2010-1622 用的 jar

CVE-2010-1622 攻击条件：

> 1. springmvc（准确来说是 spring-beans） 和 tomcat 的版本有要求
> 2. 必须要能运行 jsp
> 3. 必须要有一个 jsp 当中使用了 `taglib` 标签，并且这个 jsp 此前都没有被访问过（jsp 只会编译一次）
> 4. 必须要有一个路由方法，其参数的类型非String、prime type 