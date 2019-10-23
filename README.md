Minimal example using scala plugin with gradle 6.0-rc-1 and
scala 2.13.1. Fails with:

```
$ ./gradlew run

> Task :compileScala FAILED
java.lang.NoSuchMethodError: scala.tools.nsc.Settings.nowarn()Lscala/tools/nsc/settings/AbsSettings$AbsSetting;
xsbt.Command$.getNoWarn(Command.scala:42)
xsbt.DelegatingReporter$.apply(DelegatingReporter.scala:23)
xsbt.CachedCompiler0.<init>(CompilerInterface.scala:85)
xsbt.CompilerInterface.newCompiler(CompilerInterface.scala:28)
...
```
