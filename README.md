# Swiflicense

A Swift command line tool for generating a license for an open source project, right from your terminal.

## Installation

### Prerequisites
- [Swift](https://www.swift.org/download/)

### Installation Steps
1. Clone the repository:

```
git clone https://github.com/ishaanbedi/swiflicense.git
```

2. Navigate to the repository directory:

```
cd swiflicense
```

3. Compile and install the tool:
```
swift build -c release
swift install
```
4. Move the binary file to a directory included in the system path:
```
mv .build/release/swiflicense /usr/local/bin/swiflicense
```

On macOS, the `/usr/local/bin` directory is typically included in the default system path. 

On Linux, the recommended directory for system executables is `/usr/bin`.

After moving the binary file to a directory that is included in your system path, you can use the `swiflicense` command from any directory on your system. 

You may need to restart your terminal or log out and log back in for the changes to take effect.

### Install using a single command
To install Swiflicense, compile the tool, and include it in the system path in a single command, run the following:

```
git clone https://github.com/ishaanbedi/swiflicense.git && 

cd swiflicense && swift build -c release && 

swift install && mv .build/release/swiflicense /usr/local/bin/swiflicense
```
On macOS, this will clone the repository, navigate to the repository directory, compile and install the tool, and move the binary file to the /usr/local/bin directory, which is included in the default system path.

On Linux, the command will be similar, but the binary file will be moved to the /usr/bin directory instead.


## Usage

```
swiflicense -n NAME -y YEAR -t TYPE
```

This generates a license for the given `NAME`, `YEAR`, and `TYPE`.

### Options

```
-h            Shows this usage information.
-n NAME       The name to include in the license.
-y YEAR       The year to include in the license.
-t TYPE       The license type to generate.
```

### Available License Types
- `unlicense`
- `boost`
- `mit`
- `apache`
- `mozilla`
- `gpl`

### Example
To generate an MIT license for the year 2020 with your name, run the following command:

```
swiflicense -n "Ishaan Bedi" -y 2020 -t mit
```

### Demo
Check out this short demo of Swiflicense in action:

<img src="https://kcldtzblfykiwwltfouv.supabase.co/storage/v1/object/public/github-gif/swiflicense_demo.gif"/>



This will generate a license file named LICENSE in the current directory.

### License
This project is licensed under the MIT license.