.PHONY: build

build:
	python setup.py build_ext -i
	pythran -v call_capsule_pythran.py

_cleanso:
	rm -f *.so

clean: _cleanso
	rm -f rect.cpp rect.h
	rm -rf build

test:
	python -Wall test.py
