Building the Java Development Kit (JDK) requires that you already have a JDK for your target operating system and architecture. The JDK used to build the JDK is called the *Boot JDK*. Furthermore, the minimum version required for the Boot JDK is either the previous version, or for an early-access build, the most recently released version.

This project builds packages of JDK 18, 19, 20, and 21 for the stable, candidate, beta, and edge channels in the Snap Store. Its sole purpose is to provide a chain of trusted builds starting from JDK 17 in Ubuntu 18.04 LTS through to JDK 21 for use by the [OpenJFX Snap](https://snapcraft.io/openjfx) package to build JavaFX. The JavaFX build requires JDK 21 and cannot yet be built on the current release of JDK 22.

The full build chain of JDK 18, 19, 20, and 21 on Ubuntu 18.04 LTS is shown below:

```
Ubuntu OpenJDK 17 (openjdk-17-jdk-headless)
    ↳ Snap OpenJDK 18 (bootjdk/latest/stable)
        ↳ Snap OpenJDK 19 (bootjdk/latest/candidate)
            ↳ Snap OpenJDK 20 (bootjdk/latest/beta)
                ↳ Snap OpenJDK 21 (openjdk/latest/edge)
```

## Installation

These Snap packages are not maintained for end users. Install the [OpenJDK Snap](https://snapcraft.io/openjdk) package for the current general-availability release and early-access builds of OpenJDK.

## License

This project is licensed under the GNU General Public License v2.0 with the Classpath exception, the same license used by Oracle for the OpenJDK project. See the files [LICENSE](LICENSE) and [ADDITIONAL_LICENSE_INFO](ADDITIONAL_LICENSE_INFO) for details.

Java and OpenJDK are trademarks or registered trademarks of Oracle and/or its affiliates. See the file [TRADEMARK](TRADEMARK) for details.
