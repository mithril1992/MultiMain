Multi main project
===

Kotlinで複数の`main`を持つjarを作成するサンプル

fatJarの作成には、shadowJarを使用

例
---

``` bash
$ ./gradlew shadowJar
$ java -classpath build/libs/multi-main-1.0-SNAPSHOT-all.jar io.github.mithril1992.main.Main
$ java -classpath build/libs/multi-main-1.0-SNAPSHOT-all.jar io.github.mithril1992.sub.Main
```