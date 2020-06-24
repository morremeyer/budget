## Setup

You need to install all requirements from requirements.txt and have a config file that specifies a secret key.

### Setup the venv

```sh
python3 -m venv venv
source venv/bin/activate

pip install -r requirements.txt

# For development only
pip install -r requirements-dev.txt
```

### Configure the application

For budget to run, you need to configure it. The supplied [`settings.example.ini`](src/settings.example.ini) lists
all possible settings.

Put your configuration file at `src/settings.ini`.

You need to set at least a `SECRET_KEY` or budget will not start.
