# Test Driven Development

## Type of testing

- Unit Testing
- Development focused on test

### Modules used to test

- PyTest (`pip install pytest`)
- UnitTest (included with python)

## Why TDD

TDD helps to minimise the risk of a failure. It increases the quality of a product and reduces the chance of sending faulty/broken product to production.

## Implementation

- File for testing
- File for code
- Run the tests
- Alter the code if test fails
- Run tests again until they pass

![TDD](tdd.jpg)

## Commands

- `python -m pytest` => Runs the test
- `python -m pytest -v` => Breakdown of the test
- `python -m unittest discover -v` => Breakdown of the test

## Naming conventions

Example:

- `simple_calc` => Main file
- `test_simple_calc` => Tested file

## Example implementation

```python
class TestCalc(unittest.TestCase):
    calc = SimpleCalc()

    def test_add(self):
        self.assertEqual(self.calc.add(2, 4), 6)
```

## Example Output

```bash
================================================= test session starts =================================================
platform win32 -- Python 3.9.0, pytest-6.1.2, py-1.9.0, pluggy-0.13.1
rootdir: .\Python-Test-Driven-Development
collected 4 items

test_simple_calc.py ....                                                                                         [100%]

================================================== 4 passed in 0.04s ==================================================
```
