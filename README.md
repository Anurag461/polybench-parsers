# Polybench Parsers

A comprehensive collection of test output parsers for various programming languages and testing frameworks.

## Features

- **Multi-language Support**: Parsers for Java, Python, JavaScript, and TypeScript
- **Framework Coverage**: Support for Maven, PyUnit, Jest, Mocha, and more
- **Standardized Output**: Consistent parsing results across all frameworks
- **Easy Integration**: Simple API for integrating into your testing workflows

## Supported Frameworks

### Java
- Maven Surefire (JUnit)

### Python
- PyUnit

### JavaScript
- Jest
- Mocha

### TypeScript
- Jest
- Mocha
- Bazel Angular

## Installation

```bash
pip install polybench-parsers
```

Or with uv:

```bash
uv pip install polybench-parsers
```

## Quick Start

```python
from polybench_parsers import JavaGenericParser, PythonPyUnit

# Parse Java Maven test output
java_parser = JavaGenericParser(maven_output)
java_results = java_parser.parse()

# Parse Python PyUnit test output
python_parser = PythonPyUnit(pyunit_output)
python_results = python_parser.parse()

print(f"Passed: {java_results['num_tests_passed']}")
print(f"Failed: {java_results['num_tests_failed']}")
```

## Development

```bash
# Clone the repository
git clone https://github.com/yourusername/polybench-parsers.git
cd polybench-parsers

# Install in development mode
pip install -e .

# Run tests
pytest
```

## License

This project is licensed under the CC-BY-NC-4.0 License.
