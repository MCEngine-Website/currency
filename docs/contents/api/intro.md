# 💱 Economy API

An extensible API for handling economy balances, transactions, and formatting in Java.  
Available on GitHub Packages for seamless integration.

---

## 📦 Installation

### 🔧 Maven

```xml
<dependency>
  <groupId>io.github.mcengine</groupId>
  <artifactId>economy-api</artifactId>
  <version>{version}</version>
</dependency>
```

### ⚙️ Gradle

#### Groovy DSL

**Short form**:
```groovy
implementation 'io.github.mcengine:economy-api:{version}'
```

**Long form**:
```groovy
dependencies {
    implementation group: 'io.github.mcengine', name: 'economy-api', version: '{version}'
}
```

#### Kotlin DSL

**Short form**:
```kotlin
implementation("io.github.mcengine:economy-api:{version}")
```

**Long form**:
```kotlin
dependencies {
    implementation(group = "io.github.mcengine", name = "economy-api", version = "{version}")
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
    <url>https://maven.pkg.github.com/MCEngine-API/economy</url>
  </repository>
</repositories>
```
</details>

<details>
<summary>📚 Gradle (Groovy)</summary>

```groovy
repositories {
    maven {
        url = uri("https://maven.pkg.github.com/MCEngine-API/economy")
    }
}
```
</details>

<details>
<summary>📚 Gradle (Kotlin)</summary>

```kotlin
repositories {
    maven {
        url = uri("https://maven.pkg.github.com/MCEngine-API/economy")
    }
}
```
</details>
