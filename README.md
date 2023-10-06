# 🗂CSV ️

This is a micro library I wrote for one of my projects and then decided to share with awesome Kotlin community. It mainly covers my needs and has no documentation. Feel free to add a PR is you miss anything.

# Usage

In libs.version.toml
```toml
[versions]
csv = "0.2"

[libraries]
csv = { module = "de.halfbit:csv", version.ref = "csv" }
```

In build.gradle.kts
```kotlin
kotlin {
    sourceSets {
        val commonMain by getting {
            dependencies {
                implementation(libs.csv)
            }
        }
    }
}
```

# Release

1. Bump version in `build.gradle.kts` of the root project
2. `./gradlew clean build publishAllPublicationsToCentralRepository`

# Release Notes

- 0.2 Initial release

# License
```
Copyright 2023 Sergej Shafarenka, www.halfbit.de

You are free to
  - copy and redistribute the material in any medium or format;
  - remix, transform, and build upon the material;
  - use the material or its derivative for commercial purposes.

Any distributed derivative work containing this material or its 
parts (also if modified) must have the attribution notices in form 
of this license agreement in it.   

The material is distributed on an "AS IS" BASIS, WITHOUT WARRANTIES 
OR CONDITIONS OF ANY KIND, either express or implied.

Contact the developer if you want to use the material under a 
different license.
```
