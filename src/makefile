.PHONY: install build test clean

# Install in development mode
install:
	pip install -e .

# Build the package
build:
	python -m build

# Test the package
test:
	python test_example.py

# Clean build artifacts
clean:
	rm -rf dist/ build/ *.egg-info/

# Install dependencies
deps:
	pip install build twine pytest

# Upload to PyPI (for later)
upload-test:
	python -m twine upload --repository testpypi dist/*

upload:
	python -m twine upload dist/*