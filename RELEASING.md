# Releasing a `pyhector` version to PyPI

## Changelog

Make sure the [changelog](CHANGELOG.rst) is updated with the latest note-worthy
changes.

## Tag a Release

`pyhector` uses a "v<major>.<minor>.<patch>" format, for example:

    git tag v1.0.0

## Testing on TestPyPI

Run

    make publish-on-testpypi

and then

    make test-testpypi-install

to publish and test `pyhector` on PyPI's testing instance.

Once done the releases can be removed from the testing instance on
https://testpypi.python.org/

## Publish on PyPI

Make sure the last commit in the repository is the tagged one.

Then, run

    make publish-on-pypi

and then

    make test-pypi-install

to publish and test `pyhector` on PyPI.


## Notebook

Make sure the Jupyter Notebook is up-to date with the latest version. The
notebook can be re-compiled at
<http://mybinder.org/>.
