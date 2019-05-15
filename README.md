# demo-archetype
单模块脚手架

maven是一个很好的代码构建工具，采用“约定优先于配置”的原则进行项目管理，相信很多的java开发者应该都了解maven并可能在工作当中都是通过maven来管理项目的，在创建的项目的时候，我们往往会使用maven内置的项目骨架也就是archetype来快速生成项目结构。但是在一个团队做开发的过程中，可能仅仅依靠maven预先提供的archetyp可能是不够的，团队之间协作有自己的定义方式，每个人的结构定义风格也不尽相同，在这样的背景下我们有必要去定义一个统一的代码骨架供团队使用，这样做的好处是当团队需要开始一个新项目的时候，可以利用自定义的maven骨架一键生成项目。

　　archetype是在maven-archetype-plugin插件执行generate目标的时候进行配置的，我们经常使用到maven的内嵌的骨架包括：maven-archetype-webapp、maven-archetype-quickstart。前者用来快速搭建一个web工程项目，后者用来快速搭建一个普通的java工程项目。

   demo-archetype
        ├── pom.xml
        └── src
            └── main
                └── resources
                    ├── archetype-resources
                    │   ├── src
                    │   │   ├── main
                    │   │   │   └── java
                    │   │   │        └── Demo.java                    │   │   └── test
                    │   │       └── java
                    │   │           └── Demo.java
                    │   └── pom.xml
                    └── META-INF
                        └── maven
                            ├── archetype.xml
                            └── archetype-metadata.xml
