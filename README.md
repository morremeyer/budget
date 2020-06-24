# budget

budget is an envelope method budgeting solution for personal finance that aims to being usable both from your phone and in any desktop web browser so that you can update your expenses as you go.

If you just want to get started, see [the quick start documentation](docs/01-quickstart.md) that makes use of Docker. If you don’t want to use Docker, see the [detailed setup guide](02-setup.md)

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
