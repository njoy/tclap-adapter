# tclap-adapter
An adapter repository to plug the TCLAP header-only library into the NJOY21 build system 

## Git Subtree
This repository uses a git subtree for the directory `src`. The remote from which the subtree is made is located at [https://github.com/TCLAP/tclap.git](https://github.com/TCLAP/tclap.git). Equivalently, you can use the ssh location at `git@github.com:TCLAP/tclap.git`

To facilitate updating the subtree when it gets updated upstream, do the following:

```bash
# This only needs to be done once
git remote add TCLAP https://github.com/TCLAP/tclap.git

# Do this when you need to update the subtree
git subtree pull --prefix=src TCLAP master
```

# License
The code contained in this repository is covered by the license contained in the [LICENSE](LICENSE) file. The code in the `src` directory is covered by its own [LICENSE](src/COPYING).
