<div align="center">
<h1>toc</h1>

[toc](https://github.com/ycd/toc) TOC, table of content generator for Markdown files


![toc gif](assets/toc.gif)

</div>


# Table of Contents

- [Usage](#usage)
- [Installation](#installation)
    - [Packages](#packages)
    - [Downloads](#downloads)
    - [Compilation](#compilation)
- [Documentation](#documentation)
- [Licence](#licence)

---

## Usage



```sh
Usage: toc [options]
Options:
        -p, --path <path>        Path for the markdown file.
        -a, --append             Append toc after <!--toc--> or write to stdout. 
        -b, --bulleted           Write as bulleted or write as numbered list.


        -h, --help               Show this message and exit.
```

Add `<!--toc-->`  to your markdown to the place where you want to add Table of Contents. That's it.


```sh
$ toc -p path/to/markdown.md
```

Create numbered list instead of bulleted list.

```sh
$ toc -p path/to/markdown.md --bulleted=false
```

Write result to standart output instead of appending.

```sh
$ toc -p path/to/markdown.md --append=false
```

---


## Installation


### Packages

* [ ] For Arch Linux, install the [``]() package.
* [ ] For Homebrew on macOS, install the [``]() formula.


### Downloads

Binary downloads of example are available from [the releases section on GitHub](https://github.com/ycd/toc/releases/) for 64-bit Windows, macOS, and Linux targets. They contain the compiled executable.

| platform     |
| ----------- | 
| [macOS 64 Bit](https://github.com/ycd/toc/releases/download/v0.1.12/toc_0.1.12_darwin_x86_64.tar.gz)   
| [Linux 32-Bit](https://github.com/ycd/toc/releases/download/v0.1.12/toc_0.1.12_linux_i386.tar.gz) 
| [Linux ARM 64 Bit](https://github.com/ycd/toc/releases/download/v0.1.12/toc_0.1.12_linux_arm64.tar.gz)    
| [Linux 64 Bit](https://github.com/ycd/toc/releases/download/v0.1.12/toc_0.1.12_linux_x86_64.tar.gz)    
| [Windows 64 Bit](https://github.com/ycd/toc/releases/download/v0.1.12/toc_0.1.12_windows_x86_64.zip)       
| [Windows 32 Bit](https://github.com/ycd/toc/releases/download/v0.1.12/toc_0.1.12_windows_i386.zip)       



### Installation from source

0. Verify that you have Go 1.13+ installed

   ```sh
   $ go version
   ```

   If `go` is not installed, follow instructions on [the Go website](https://golang.org/doc/install).

1. Clone this repository

   ```sh
   $ git clone https://github.com/ycd/toc 
   $ cd ycd
   ```

2. Build and install

   #### Unix/Linux
   ```sh
   # May require you to use sudo
   $ go build .
   $ cp toc /usr/local/toc
   ```
3. Verify installation

   ```sh
   $ toc -h 
   Usage: toc [options]
   Options:
           -p, --path <path>        Path for the markdown file.
           -a, --append             Append toc after <!--toc-->, or write to stdout. 
           -b, --bulleted           Write as bulleted, or write as numbered list.


           -h, --help               Show this message and exit.
   ```
---


## Contributing

All kinds of Pull Requests and Feature Requests are welcomed!

## Licence

toc's source code is licenced under the [Apache 2.0 License](https://www.apache.org/licenses/LICENSE-2.0.txt).
