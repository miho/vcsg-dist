# vcsg-dist

[ ![Download](https://api.bintray.com/packages/miho/JCSG/vcsg-dist/images/download.svg) ](https://bintray.com/miho/JCSG/vcsg-dist/_latestVersion)

VCSG binary distribution (contains occ-csg and other native tools). 

## How to Build vcsg-dist

### Requirements

- Java >= 1.8
- Internet connection (dependencies are downloaded automatically)
- IDE: [Gradle](http://www.gradle.org/) Plugin (not necessary for command line usage)
- local ugshell executable and lua scripts that shall be added to the distribution

### IDE

Open the `vcsg-dist` [Gradle](http://www.gradle.org/) project in your favourite IDE (tested with NetBeans 8.2) and build it
by calling the `assemble` task.

### Command Line

Navigate to the [Gradle](http://www.gradle.org/) project (e.g., `path/to/vcsg-dist`) and enter the following command

#### Bash (Linux/OS X/Cygwin/other Unix-like shell)

    sh gradlew assemble
    
#### Windows (CMD)

    gradlew assemble
    
### Distribution Layout

Distributions layout looks as follows:

```
.
├── LICENSE
├── README.md
├── THIRDPARTY-LICENSES
└── bin
    └── occ-csg[.exe]
            
```
Distributions are are packaged as `vcsg.zip`. The locations for distributions are:

```
.
│
└── src
    └── eu
        └── mihosoft
            └── vcsg
                └── vcsgdist
                    ├── linux
                    │   ├── x64/vcsg.zip
                    │   └── x86
                    │
                    ├── osx/vcsg.zip
                    │   
                    └── windows
                        ├── x64
                        │   └── vcsg.zip
                        └── x86
```
