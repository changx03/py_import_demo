# Example on relative import

## Solution 1: Run the Script as a Module

```bash
python -m app.main
```

## Solution 2: Modify the PYTHONPATH

On Linux:

```bash
export PYTHONPATH=$(pwd)
python app/main.py
```

On Windows (cmd)

```bash
set PYTHONPATH=%cd%
python app\main.py
```

## Solution 3: Use Absolute Import

```python
from app.utils.math_utils import print_sqrt2
```

## Build wheel in Conda on Windows

```bash
python -m build --no-isolation
python -m pip install .\dist\import_demo-0.1.0-py3-none-any.whl
```
