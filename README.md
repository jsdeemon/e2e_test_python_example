
# Python E2E Test Example


### These Tests:
* run python selenium e2e tests against an existing website
* make use of a page object pattern
* use [pytest](http://pytest.org/) for most of the heavy lifting
* run on Firefox or Chrome
* run tests in parallel (via [pytest-parallel](https://pypi.org/project/pytest-parallel/) (requires python3.6+)
* run api tests using [requests](http://docs.python-requests.org/en/master/)
* run on merge on [CI](https://app.codeship.com/projects/312669)

## Getting started
```bash
$ virtualenv venv
$ source venv/bin/activate
```

## Install
1. install requirements: `pip install -r requirements.tx`
1. if you want to run on firefox, [download geckodriver](https://github.com/mozilla/geckodriver/releases) and move to a folder on your path (eg. `/usr/local/bin`)

## Run Tests
1. in Chrome (default): `pytest`
1. in Firefox `pytest --driver firefox`
1. in parallel `pytest --workers 2`
