Building the JDK (Java Development Kit) requires that you already have a JDK for your target operating system and architecture. The JDK used to build the JDK is called the *Boot JDK*. Furthermore, the minimum version required for the Boot JDK is either the previous version, or for an early access build, the most recently released version.

This project builds packages of OpenJDK 12, 13, and 14 for the candidate, beta, and edge channels in the Snap Store. Its sole purpose was to provide a chain of trusted builds from OpenJDK 11 in Ubuntu 18.04 LTS through to OpenJDK 15 in the initial release of the [OpenJDK Snap](https://snapcraft.io/openjdk) package.

The full chain of trusted builds in creating OpenJDK 15 is shown below:

```
Ubuntu 18.04 LTS with GLIBC 2.27 (core18 base)
Ubuntu OpenJDK 11 (openjdk-11-jdk-headless)
    ↳ Snap OpenJDK 12 (bootjdk/latest/candidate)
        ↳ Snap OpenJDK 13 (bootjdk/latest/beta)
            ↳ Snap OpenJDK 14 (bootjdk/latest/edge)
                ↳ Snap OpenJDK 15 (openjdk/latest/candidate → stable)
                    ↳ Snap OpenJDK 16 (openjdk/latest/beta)
                    ↳ Snap OpenJDK 17 (openjdk/latest/edge)
```

## Install

OpenJDK 12, 13, and 14 are no longer maintained by Oracle or any other Java vendor. For the latest General-Availability Release and Early-Access Builds of OpenJDK, please see the [OpenJDK Snap](https://snapcraft.io/openjdk) package in the Snap Store.

## License and Trademarks

This project is licensed under the GNU General Public License v2.0 with the Classpath exception, the same license used by Oracle for the OpenJDK project. See the files [LICENSE](LICENSE) and [ADDITIONAL_LICENSE_INFO](ADDITIONAL_LICENSE_INFO) for details.

Java and OpenJDK are trademarks or registered trademarks of Oracle and/or its affiliates. See the file [TRADEMARK](TRADEMARK) for details.
