# Reproduction Of scalafmt Issue [3762](https://github.com/scalameta/scalafmt/issues/3762)

View `alignment.scala` and see:

```scala
object C {
  case object B  extends A
  case object BB extends A
}
```

Run `scalafmt` (assumes `scalafmt` CLI is installed and using version `3.7.17`)

See `alignment.scala` reformatted to remove alignment from `extends`:

```scala
object C {
  case object B extends A
  case object BB extends A
}
```