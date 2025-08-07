# Application Builder

**I made Application Builder with the help of Jehovah!**

Application Builder is an application to make C applications easily, with other programming languages!

How to install:

```bash
echo "Installing AB.."
echo "We need sudo permissions to install AB."
sudo -v
wget https://raw.githubusercontent.com/zer0users/ab/refs/heads/main/ab -O ab
sudo mv ab /usr/bin/ab
echo "AB Installed succefully! Execute it with 'ab' on the terminal."
```

Project example:

```structure
MyApp
> app.py
> Buildfile
```

app.py:

```python
print('Welcome to my App!')
```

Buildfile:

```ab
INCLUDE app.py
CONFIG "init" "python3"
CONFIG "init_file" "app.py"
BUILD IMAGE
COMPILE IMAGE
```

How to compile:

```bash
ab build
```

On the directory.
