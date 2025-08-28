# 💲 Economy Common

Common utilities and shared components for the Economy API module.  
Available through GitHub Packages for easy dependency management.

---

## 📦 Installation

### 🔧 Maven

```xml
<dependency>
  <groupId>io.github.mcengine</groupId>
  <artifactId>economy-common</artifactId>
  <version>{version}</version>
</dependency>
```

### ⚙️ Gradle

#### Groovy DSL

**Short form**:
```groovy
implementation 'io.github.mcengine:economy-common:{version}'
```

**Long form**:
```groovy
dependencies {
    implementation group: 'io.github.mcengine', name: 'economy-common', version: '{version}'
}
```

#### Kotlin DSL

**Short form**:
```kotlin
implementation("io.github.mcengine:economy-common:{version}")
```

**Long form**:
```kotlin
dependencies {
    implementation(group = "io.github.mcengine", name = "economy-common", version = "{version}")
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
    <url>https://maven.pkg.github.com/MCEngine-Common/economy</url>
  </repository>
</repositories>
```
</details>

<details>
<summary>📚 Gradle (Groovy)</summary>

```groovy
repositories {
    maven {
        url = uri("https://maven.pkg.github.com/MCEngine-Common/economy")
    }
}
```
</details>

<details>
<summary>📚 Gradle (Kotlin)</summary>

```kotlin
repositories {
    maven {
        url = uri("https://maven.pkg.github.com/MCEngine-Common/economy")
    }
}
```
</details>
