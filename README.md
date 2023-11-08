# Code coverage is a lie

*A principle example to show that code coverage is a bad indicator of software quality*

### Test coverage

```
❯ python -m pytest --cov
======================= test session starts ====================
platform darwin -- Python 3.11.5, pytest-7.4.2, pluggy-1.3.0
rootdir: /Users/emil/Development/code-coverage-is-a-lie
plugins: cov-4.1.0
collected 1 item

tests/test_calc.py .                                                                                                                                                         [100%]

---------- coverage: platform darwin, python 3.11.5-final-0 ----------
Name                 Stmts   Miss  Cover
----------------------------------------
calc/__init__.py         0      0   100%
calc/calc.py             2      0   100%
tests/test_calc.py       3      0   100%
----------------------------------------
TOTAL                    5      0   100%


======================== 1 passed in 0.08s =====================
```

### Output

```python
from calc.calc import add

print(add(5, 10)) # => "510"
```
