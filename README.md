## qcheck

A script to display user quota info graphically on the terminal


This is just a wrapper script around quota -a, therefore quota should be installed and users should have access to it


## Contributing

After making a change you will have to bump the version in setup.cfg for the package to build automatically with git


## Install with pip from git package repo

To install you will need access to the project and use your personal access token

```bash
pip3 install --upgrade qcheck --extra-index-url https://__token__:<REDACTED>@gitlab.computing.dcu.ie/api/v4/projects/10226/packages/pypi/simple
```

This should automatically install the qcheck command to `/usr/local/bin/qcheck`


## Install and build locally

```bash
git clone $repo
pip3 install build
apt install python3-virtualenv

cd $repo
python3 -m build 
pip3 install dist/qcheck...*...whl
```

