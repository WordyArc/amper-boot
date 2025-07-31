# Amper Boot

Amper Boot is a template for quickly starting a Spring Boot project using the JetBrains Amper build system.

With it you don’t have to dig into bulky Maven XML configurations or rewrite complex Gradle scripts: just clone the repository and run a couple of commands.

## Why Amper?

- **Simple configuration.** Unlike Maven’s bulky XML and Gradle’s complex DSL, Amper uses an intuitive YAML format.
- **Fast builds.** Incremental mode and caching speed up builds even for very large projects.
- **Native IDE support.** Excellent integration with IntelliJ IDEA and Fleet.

## Links

- JetBrains Amper (GitHub): https://github.com/JetBrains/amper
- JetBrains Amper (Blog): https://blog.jetbrains.com/amper/
- Spring Boot (Official site): https://spring.io/projects/spring-boot
- Spring Boot (Documentation): https://docs.spring.io/spring-boot/docs/current/reference/html/

## Requirements

- JetBrains Amper version ≥ 0.7.0
- Java Development Kit (JDK) version ≥ 17
- IntelliJ IDEA 2025.1.2 Preview or later (recommended)

## Quick Start

1. Clone the repository and navigate into the project folder:

```shell
   git clone https://github.com/wordyarc/amper-boot.git
   cd amper-boot
```

2.	Build and run the application:

```shell
./amper build
./amper run
```

## Configuration

In the module.yaml file you can configure:
- product: module type (jvm/app, jvm/lib, etc.).
- springBoot: enables Spring Boot support.
- dependencies: list of dependencies.
- test-dependencies: dependencies for testing.
- settings: BOM, JDK version, and other options.

all options [DSL documentation](https://github.com/JetBrains/amper/blob/release/0.7/docs/DSLReference.md)
## Amper Commands

To see the list of all commands and options:

```shell
./amper --help
```

Frequently used commands:

```shell
./amper init    # create a new Amper project.
```

```shell
./amper build   # compile and build all modules.
```

```shell
./amper test    # run tests.
```

```shell
./amper run     # run the application.
```

```shell
./amper clean   # remove artifacts and caches.
```

## Updating Amper

To update the wrapper scripts and CLI distribution:

```shell
./amper update
```

Add the --dev option if you want to try pre-release (dev) builds.

## Contributing

PRs are welcome!

## License

This project is licensed under the Apache License 2.0. See [LICENSE](LICENSE) for details.
