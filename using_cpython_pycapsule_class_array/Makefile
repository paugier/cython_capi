.PHONY: build

build:
	python setup.py build_ext -i
	pythran -v call_capsule_pythran.py

_cleanso:
	rm -f *.so

clean: _cleanso
	rm -f *.cpp
	rm -f *api.h
	rm -rf build

test:
	python -Wall test.py

all: clean build test
