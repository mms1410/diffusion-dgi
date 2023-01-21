
## Steps to build documentation

1. Build and install package from source.
```bash
cd ./diffusion-dgi/
pip install -e .
pip install sphinx sphinx_rtd_theme sphinx_copybutton
```

2. Generate documentation from your docstrings.
```bash
cd docs/
sphinx-apidoc -f -o ./source ../src/diffusion-dgi
```
3. Build the documentation
```bash
make clean && make html
```
4. You can now view your documentation under `docs/build/html/index.html`.
