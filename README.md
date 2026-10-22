Building the Java Development Kit (JDK) requires that you already have a JDK for your target operating system and architecture. The JDK used to build the JDK is called the *Boot JDK*. Furthermore, the minimum version required for the Boot JDK is either the previous version, or for an early-access build, the most recently released version.

This project builds packages of JDK 25, 26, 27, and 28 for the stable, candidate, beta, and edge channels in the Snap Store. Its sole purpose is to provide a chain of trusted builds starting from JDK 25 through to JDK 28 for use in building the [OpenJDK](https://snapcraft.io/openjdk) and [OpenJFX](https://snapcraft.io/openjfx) Snap packages.

## Installation

The BootJDK Snap package is not intended for external use. Install the [OpenJDK Snap](https://snapcraft.io/openjdk) package for the current general-availability release and early-access builds of OpenJDK.

## License

This project is licensed under the GNU General Public License v2.0 with the Classpath exception, the same license used by Oracle for the JDK project. See the files [LICENSE](LICENSE), [ADDITIONAL_LICENSE_INFO](ADDITIONAL_LICENSE_INFO), and [ASSEMBLY_EXCEPTION](ASSEMBLY_EXCEPTION) for details.

Java and OpenJDK are trademarks or registered trademarks of Oracle and/or its affiliates. See the file [TRADEMARK](TRADEMARK) for details.
