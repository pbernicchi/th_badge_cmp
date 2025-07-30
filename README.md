## Telehack Badge Compare-er 🤷‍♂️

A simple script to compare badges for two Telehack users.  Uses the `/u/username.json` API, rather than the older HTML user page `/u/username` URL.

### Requirements

For local (system-managed) Python installations: run `pip3 install requests` prior to running the script per "Usage."

⚠️ Consider using a virtual environment (venv) if you are using an externally-managed Python3 installation such as via Homebrew for macOS, as outlined below:

```
cd /path/to/this/local/repo
python3 -m venv venv
source venv/bin/activate
```
This will create a new Python virtual environment (venv) and activate it, which should change your shell prompt as a reminder.

Next,

`pip3 install requests`

The last line will install the `requests` module, along with its dependencies, which are:

```
certifi==2025.7.14
charset-normalizer==3.4.2
idna==3.10
requests==2.32.4
urllib3==2.5.0
```
You can verify successful installation if you wish by running `pip3 freeze`.

Now, deactivate the virtual environment:
`deactivate`

Then, modify `th_badge_cmp.py`, replacing the existing shebang to reflect the virtual environment we just created:
`#!/home/user/myproject/venv/bin/python`

Finally, save the file. Oh, the things we Mac users have to deal with! Seriously though, a virtual environment is the best way to do this if you installed Python3 with Homebrew.


### Usage:
```
  $ ./th_badge_cmp.py <user1> <user2>
```

### Contributing:
Pull requests are welcome but if you created a virtual Python3 environment using the instructions above, kindly restore the original shebang until I can work out a more universal solution:
`#!/usr/bin/env python3`

### Credits:

- **drsleepy** [Telehack](https://telehack.com/u/drsleepy) | [GitHub](https://github.com/drsleepy1)
    - Original script creator; I originally forked and tried to submit a PR with these improvements but they fell into limbo.

- **pbernicc** [Telehack](https://telehack.com/u/pbernicc) | [GitHub](https://github.com/pbernicchi)
    - Added colours, made use of the JSON endpoint

- **underwood** [Telehack](https://telehack.com/u/underwood) | [GitHub](https://github.com/thunderpoot)
    - Pushed it through the Pylint cheese-cloth
