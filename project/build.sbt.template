import scalariform.formatter.preferences._

lazy val root = (project in file(".")).
  settings(commonSettings: _*).
  settings(
    name := "SampleProject",
    libraryDependencies ++= Seq()
  )

lazy val commonSettings = Seq(
  organization := "your.organization",
  version := "0.1.0",
  // build.sbt supports 2.10.x only due to scalariform version. Use Build.scala for 2.11.x
  scalaVersion := "2.10.4",
  scalacOptions ++= Seq("-unchecked", "-deprecation"),
  javacOptions ++= Seq("-source", "1.6", "-target", "1.6"),
  resolvers ++= Seq(
    "Sonatype OSS Releases" at "https://oss.sonatype.org/content/repositories/releases",
    "Sonatype OSS Snapshots" at "https://oss.sonatype.org/content/repositories/snapshots",
    "Typesafe Releases" at "http://repo.typesafe.com/typesafe/releases/"
  )
)


// scalariform code format settings
scalariformSettings // enable scalariformSettings

ScalariformKeys.preferences := ScalariformKeys.preferences.value
  .setPreference(RewriteArrowSymbols, false)
  .setPreference(AlignParameters, true)
  .setPreference(AlignSingleLineCaseStatements, true)
  .setPreference(DoubleIndentClassDeclaration, true)
  .setPreference(IndentSpaces, 2)

