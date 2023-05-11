# Steamship Package Template 

This repository contains a starter template showing you how to develop and use a package.

## Quick Start

Deploy and use this package in under a minute!

First, make sure you have the Steamship CLI installed:

```bash
   git clone https://github.com/steamship-packages/empty-package.git my-new-package
   cd my-new-package
   pip install -r requirements.txt
```

Then, deploy your package!

```bash
ship deploy
```


### Invoke your Package from Python

It's more likely you'll want to call your package from software you're writing. Let's try from Python.

Create a new instance and invoke it with:

```python
from steamship import Steamship

# TODO: Replace with your package and instance handle below
instance = Steamship.use("PACKAGE_HANDLE", "INSTANCE_HANDLE", config={
    "default_name": "Beautiful"
})

print(instance.invoke("greet"))
```

## Extending on your own

Steamship packages run on a cloud stack designed for AI.

You can import files, parse and tag them, query over them, and return custom results. 

Full documentation for developers is available at [https://docs.steamship.com/packages/developing](https://docs.steamship.com/packages/developing).
