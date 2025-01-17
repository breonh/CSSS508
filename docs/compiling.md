
# Compiling R Packages

The newest versions of R packages are often available only as source code. When you install or update the package, it may indicate it needs compilation. To enable your computer to compile the code in these packages, you need to do a small amount of additional setup. Before you start, make sure R is closed. I recommend rebooting after installing, as well, but it is not a requirement.

## Mac

On a Mac, you only need to install Xcode Command Line Tools. This is simple:

1. Open a terminal window
   * Click Spotlight search in the top right of your screen, then search for "Terminal"


2. Copy and paste the following into the terminal, then press enter.
```
xcode-select --install
```

3. You will probably need to provide your password to enable installing the software.

4. Follow any onscreen instructions and wait for it to finish.

5. You can now compile R packages!

## Windows

On a PC, you need to obtain a toolchain for compiling. The easiest way to do this is with RTools:

1. [Browse to this page](https://cran.r-project.org/bin/windows/Rtools/).

2. Download the newest 64-bit Rtools installer.

3. Run the file to install, following all onscreen instructions. If you are unsure about anything, leave the default settings.

4. [Go back to this page](https://cran.r-project.org/bin/windows/Rtools/). Follow the remaining instructions. But, first, run `Sys.which("make")` and see if it finds a `make.exe` file. If so, you're good to go. If not, do the path stuff.

5. You can now compile R packages!

# Troubleshooting

Compiling code is complicated and sometimes errors specific to your machine will arise even if you followed everything above correctly. Reach out if you have issues!