# netupload

<br>
<a href="https://pypi.org/project/netupload/">
    <img src="https://img.shields.io/pypi/v/netupload" alt="PyPI - Version">
</a>
<a href="https://github.com/zpg6/netupload">
    <img src="https://img.shields.io/pypi/l/netupload" alt="PyPI - License">
</a>
<a href="https://github.com/zpg6/netupload">
    <img src="https://img.shields.io/badge/github-zpg6/netupload-black" alt="GitHub Repo">
</a>
<br><br>

Simple file upload server for when you need to send files around on your local network.
Sometimes you don't want to login to your email and don't have a USB so this can be a quick way to transfer files.

![How it works](https://github.com/zpg6/netupload/raw/main/docs/how_it_works.png)

## Usage

Install the package:

```
pip install netupload
```

Start the server with the default options:

```
netupload
```

## Options

```
netupload --host=0.0.0.0 --port=4000 --save-dir=./uploads
```

| Option     | Description                      | Default   |
| ---------- | -------------------------------- | --------- |
| --host     | Host to run the server on        | 0.0.0.0   |
| --port     | Port to run the server on        | 4000      |
| --save-dir | Directory to save uploaded files | ./uploads |

## Webpage

The server runs a webpage that you can access from any device on the same network.
You will see the

```
> netupload --host=0.0.0.0 --port=4000 --save-dir=./uploads

 * Serving Flask app 'src.app'
 * Debug mode: off
 * Running on all addresses (0.0.0.0)
 * Running on http://127.0.0.1:4000
 * Running on http://192.168.1.231:4000 <--------- THIS ADDRESS WITH YOUR COMPUTER'S LOCAL IP
```

Navigate to the address shown in the terminal to access the webpage:

![Webpage Screenshot](https://github.com/zpg6/netupload/raw/main/docs/webpage_screenshot.png)
