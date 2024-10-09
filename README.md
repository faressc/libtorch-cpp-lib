# libtorch-cpp-lib

## Linux aarch64

- install all python dependencies in venv

```bash
python -m venv venv
source venv/bin/activate
pip install pyyaml pybind11 typing-extensions
```

- Follow [this guide](https://github.com/pytorch/pytorch/blob/main/docs/libtorch.rst) to install libtorch (change the python to the one in the venv when building locally)

For now on linux aarch64 kineto throws an error, so we need to disable it.

```bash
-DUSE_KINETO=OFF
```