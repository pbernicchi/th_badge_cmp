## Telehack Badge Compare-er 🤷‍♂️

A simple script to compare badges for two Telehack users. Uses the `/u/username.json` API rather than the older HTML user page.

### Requirements

Python 3 with the `requests` module. If you're on a system-managed Python (e.g. Homebrew on macOS), use a virtual environment:

```
python3 -m venv th_badge_cmp_venv
th_badge_cmp_venv/bin/pip install requests
```

For a plain system Python where `pip install` works globally:

```
pip3 install requests
```

### Usage

```
th_badge_cmp_venv/bin/python th_badge_cmp.py <user1> <user2>
```

Or, if `requests` is installed globally:

```
./th_badge_cmp.py <user1> <user2>
```

### Contributing

Pull requests are welcome.

### Credits

- **drsleepy** [Telehack](https://telehack.com/u/drsleepy) | [GitHub](https://github.com/drsleepy1)
    - Original script creator; I originally forked and tried to submit a PR with these improvements but they fell into limbo.

- **pbernicc** [Telehack](https://telehack.com/u/pbernicc) | [GitHub](https://github.com/pbernicchi)
    - Added colours, made use of the JSON endpoint

- **underwood** [Telehack](https://telehack.com/u/underwood) | [GitHub](https://github.com/thunderpoot)
    - Pushed it through the Pylint cheese-cloth
