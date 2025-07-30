# 💱 Currency API

An extensible API for handling currency exchange, conversion, and formatting in Java.  
Available on GitHub Packages for seamless integration.

---

## 📦 Installation

### 🔧 Maven

```xml
<dependency>
  <groupId>io.github.mcengine</groupId>
  <artifactId>currency-api</artifactId>
  <version>{version}</version>
</dependency>
```

### ⚙️ Gradle

#### Groovy DSL

**Short form**:
```groovy
implementation 'io.github.mcengine:currency-api:{version}'
```

**Long form**:
```groovy
dependencies {
    implementation group: 'io.github.mcengine', name: 'currency-api', version: '{version}'
}
```

#### Kotlin DSL

**Short form**:
```kotlin
implementation("io.github.mcengine:currency-api:{version}")
```

**Long form**:
```kotlin
dependencies {
    implementation(group = "io.github.mcengine", name = "currency-api", version = "{version}")
}
```

---

## 🛠 Repository Configuration (GitHub Packages)

<details>
<summary>📚 Maven</summary>

```xml
<repositories>
  <repository>
    <id>github</id>
    <url>https://maven.pkg.github.com/MCEngine-API/currency</url>
  </repository>
</repositories>
```
</details>

<details>
<summary>📚 Gradle (Groovy)</summary>

```groovy
repositories {
    maven {
        url = uri("https://maven.pkg.github.com/MCEngine-API/currency")
    }
}
```
</details>

<details>
<summary>📚 Gradle (Kotlin)</summary>

```kotlin
repositories {
    maven {
        url = uri("https://maven.pkg.github.com/MCEngine-API/currency")
    }
}
```
</details>
