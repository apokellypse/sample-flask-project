# Quick Setup Instructions

## Environment: Backend

### Note
I'm using Mac OSX. In the future, I can add more fleshed out instructions for those on Windows and Linux.

### Get Homebrew
```
/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
```

### Get pip and Flask
```
sudo easy_install pip
pip install flask
```

### Get node
```
brew install node
```

## Environment: Frontend

### Get gulp (opt.)
```
npm update minimatch
npm install event-stream
npm install --global gulp-cli
npm install --save-dev gulp
npm install --save-dev gulp-concat
npm install --save-dev gulp-uglify
npm install --save-dev gulp-sass
npm install --save-dev gulp-rename
npm install --save-dev gulp-jshint
```

### Get bootstrap (opt.)
```
npm install bootstrap@4.0.0-alpha.2
```

## Running the server locally

```python
python runserver.py
```

## Running gulp to compile sass, minify js, etc.

```
gulp
```

## Troubleshooting
* I'm using Sublime, and I don't see the `__init__.py` file.

To see the `__init__.py` file in sublime, you need to go to:  
Sublime Text > Preferences > Settings - User

and make sure that you have

```
{
	"folder_exclude_patterns": []
}
``` 

* Can't find node module...

Remove your node_modules folder, and call the following cmd:
```
npm install
```