# 📦 Go Makefile Tutorial

This repository provides a simple, clean `Makefile` for Go projects.  
It helps automate common development tasks like building, formatting, and running your Go programs.

---

## 🛠️ Features

- `make fmt` – Format all Go files
- `make vet` – Run `go vet` to find suspicious constructs
- `make build` – Compile the code and create a binary
- `make clean` – Clean up compiled files
- `make execute` – Build and run the program

---

## 🚀 How to Use

### 🔧 1. Clone the Repo
You can clone or download this repo to use the Makefile in your project:

```bash
git clone https://github.com/Alireza-Morady/make-config-go.git
```
Or, create your own Makefile:
1. In your Go project folder, create a new file named Makefile.
2. Copy the contents of the Makefile from this repository and paste it into your Makefile.

### 🛠️ 2. Initialize a Go Module
Before you can use the Makefile, you need to initialize a Go module for your project. This step is required to manage your project dependencies.

Run the following command to initialize a Go module:
```bash
go mod init <your-project-name>
```
Replace <your-project-name> with your desired project name (for example, make-config-go if you are using the same name as the repository).
> ⚠️ **Important:** The name you use for your Go module (`go mod init <your-project-name>`)  
> should match the `BINARY_NAME` variable inside your `Makefile`.  
> This ensures that the Makefile correctly builds and executes your Go project.

#### 🔄 How It Works
Once you've added the Makefile and initialized the Go module, the following commands are available:
- `make fmt`: Formats all Go source files.
- `make vet`: Analyzes code for potential issues.
- `make build`: Builds the binary based on `BINARY_NAME`.
- `make clean`: Cleans up generated files.
- `make execute`: Builds and then runs the program.

### 💻 3. Installing Make (If Not Already Installed)
If your system doesn't have make installed, you can install it based on your operating system:

For Linux:
```bash
sudo apt update
sudo apt install build-essential
```
For macOS:
```bash
brew install make
```
For Windows:
1.Download and install **Gow** (GNU on Windows) from [Gow's official website](https://github.com/bmatzelle/gow/releases).
2.fter installation, make will be available from your command prompt.

### ⚙️ 4. Customizing the Makefile  
The default binary name for the compiled Go project is Exe. If you want to change the binary name, simply modify the BINARY_NAME variable in the Makefile.

For example, to change the binary name to myapp, update the Makefile:
```
BINARY_NAME := myapp
```
After modifying the BINARY_NAME, you should ensure that the name you choose matches the name you use when running go mod init.

### 🚀 5. Running the Commands
Now that everything is set up, you can run any of the commands listed in the Makefile. For example, to build your Go project, run:
```
make build
```
Or to execute the program and do every commands instruct:
```
make
```
That's it! Your Go project is now streamlined with the Makefile configuration. Enjoy coding and developing with ease!

