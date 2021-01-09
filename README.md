## ![Duke, the Java mascot, with arms akimbo](images/icon.png) BootJDK Snap

Building the JDK (Java Development Kit) requires that you already have a JDK for your target operating system and architecture. The JDK used to build the JDK is called the *Boot JDK*. Furthermore, the minimum version required for the Boot JDK is either the previous version, or for an early access build, the most recently released version.

This project builds Snap packages of OpenJDK 12, 13, and 14, so that I can build OpenJDK 15 directly from its [GitHub repository](https://github.com/openjdk/jdk15u.git) using only the software in [Ubuntu 18.04 LTS](https://cloud-images.ubuntu.com/bionic/current/).

The full chain of trusted builds is shown below:

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

### Installation

Although you can install these Boot JDK packages, they are no longer maintained by Oracle or any other Java vendor. For the current release of OpenJDK, please see the [OpenJDK Snap](https://github.com/jgneff/openjdk) repository or its listing in the [Snap Store](https://snapcraft.io/openjdk).

### License and Trademarks

This project is licensed under the GNU General Public License v2.0 with the Classpath exception, the same license used by Oracle for the OpenJDK project. See the files [LICENSE](LICENSE) and [ADDITIONAL_LICENSE_INFO](ADDITIONAL_LICENSE_INFO) for details.

Java and OpenJDK are trademarks or registered trademarks of Oracle and/or its affiliates. See the file [TRADEMARK](TRADEMARK) for details.
