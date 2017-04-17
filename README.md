# scala-test-study

`scalastyleSources in Compile := (unmanagedSourceDirectories in Compile).value`
の一文を追加するところで、
`scalastyleSources in` と `:=` の部分が赤文字になってしまい、
Refresh projectできませんでした。

`addSbtPlugin("org.scalastyle" %% "scalastyle-sbt-plugin" % "0.6.0")`
`scalastyleSources in Compile := (unmanagedSourceDirectories in Compile).value`
それぞれで、 File > Invalidate Cache/Restart... を実行してみてもだめでした。


```
Error:Error while importing SBT project:<br/><pre>Java HotSpot(TM) 64-Bit Server VM warning: ignoring option MaxPermSize=384M; support was removed in 8.0
[info] Loading project definition from /Users/masashi/IdeaProjects/scala-test-study/project
/Users/masashi/IdeaProjects/scala-test-study/build.sbt:7: error: not found: value scalastyleSources
scalastyleSources in Compile := (unmanagedSourceDirectories in Compile).value
^
[error] Type error in expression
Invalid response.

```
