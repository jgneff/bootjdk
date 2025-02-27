Building the Java Development Kit (JDK) requires that you already have a JDK for your target operating system and architecture. The JDK used to build the JDK is called the *Boot JDK*. Furthermore, the minimum version required for the Boot JDK is either the previous version, or for an early-access build, the most recently released version.

This project builds packages of JDK 21, 22, 23, and 24 for the stable, candidate, beta, and edge channels in the Snap Store. Its sole purpose is to provide a chain of trusted builds starting from JDK 21 in Ubuntu 20.04 LTS through to JDK 24 for use by the [OpenJDK Snap](https://snapcraft.io/openjdk) package.

The full build chain of JDK 21, 22, 23, and 24 on Ubuntu 20.04 LTS is shown below:

```
OpenJDK 21 package in Ubuntu 20.04 (openjdk-21-jdk-headless)
↳ BootJDK 21 Snap (bootjdk/latest/stable)
  ↳ BootJDK 22 Snap (bootjdk/latest/candidate)
    ↳ BootJDK 23 Snap (bootjdk/latest/beta)
      ↳ BootJDK 24 Snap (bootjdk/latest/edge)
        ↳ OpenJDK 25 Snap (openjdk/latest/edge)
```

## Installation

These Snap packages are not maintained for end users. Install the [OpenJDK Snap](https://snapcraft.io/openjdk) package for the current general-availability release and early-access builds of OpenJDK.

## License

This project is licensed under the GNU General Public License v2.0 with the Classpath exception, the same license used by Oracle for the JDK project. See the files [LICENSE](LICENSE), [ADDITIONAL_LICENSE_INFO](ADDITIONAL_LICENSE_INFO), and [ASSEMBLY_EXCEPTION](ASSEMBLY_EXCEPTION) for details.

Java and OpenJDK are trademarks or registered trademarks of Oracle and/or its affiliates. See the file [TRADEMARK](TRADEMARK) for details.
