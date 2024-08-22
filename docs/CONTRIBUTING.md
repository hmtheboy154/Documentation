# Contributing to Bliss OS Documentation

We are using mkdocs for our documentation, and the setup for that is fairly easy. 
All our docs are using Markdown, so you can easily submit a PR for any existing page. 

For moe complex updates, we recommend you use mkdocs to build the site edits and verify all things work as intended. 

### Install Dependencies

Mkdocs dependencies is fairly simple and straightforward
- Python3+ 
- pip
- python venv

If you are using Debian/Ubuntu based distro:

```
sudo apt-get install python3 python3-pip python3.12-venv
```

### Clone Documentation Repo

We now need to clone the docs repo:

```
git clone git@github.com:hmtheboy154/Documentation.git Documentation
cd Documentation
git checkout origin/rework
```

### Setup Virtual Environment

Next we need to setup a venv for the site framework:

```
python3 -m venv venv
source venv/bin/activate
```

### Setup MkDocs & Theme

Next we need to install mkdocs and the Material theme we are using:

```
pip install mkdocs mkdocs-material
```

### Make Your Changes

From here we can enter the docs/ folder and start editing our markdown however needed. Then when you are eady to see how it all fits together, use the following build command:

```
mkdocs build
```

After that, you will see a "site/" folder with the index.html you can open in your browser of choice and verify your changes worked correctly. 