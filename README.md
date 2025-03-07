# Shopsite Tool

`shopsite` is a command-line tool to manage the frontend and backend services for [my shopping-site repository](https://github.com/rayhuang2006/shopping-site). This script allows you to start, stop, check the status, restart, and view logs for both frontend and backend services that run in separate screen sessions.

## Requirements

- Linux or Unix-based operating system
- `screen` installed
- `Node.js` and `npm` installed
- A local copy of the `shopping-site` repository

## Usage

### Start Services

To start the frontend and/or backend services in separate screen sessions:

```bash
./shopsite -on [--f | --b]
```

- `--f`: Start only the frontend.
- `--b`: Start only the backend.
- No option: Start both frontend and backend.

### Stop Services

To stop the frontend and/or backend services:

```bash
./shopsite -off [--f | --b]
```

- `--f`: Stop only the frontend.
- `--b`: Stop only the backend.
- No option: Stop both frontend and backend.

### Check Service Status

To check the status of the services:

```bash
./shopsite -st [--f | --b]
```

- `--f`: Show the status of the frontend.
- `--b`: Show the status of the backend.
- No option: Show the status of both frontend and backend.

### Restart Services

To restart the services:

```bash
./shopsite -re [--f | --b]
```

- `--f`: Restart only the frontend.
- `--b`: Restart only the backend.
- No option: Restart both frontend and backend.

### View Logs

To view the logs of the services:

```bash
./shopsite -log [--f | --b]
```

- `--f`: View the frontend logs.
- `--b`: View the backend logs.

### Help

To display the help menu and see a list of available commands:

```bash
./shopsite help
```

or

```bash
./shopsite -h
```

## Configuration

The script uses a configuration file located at `~/.shopsite_config` to store the path to your `shopping-site` directory. If the file does not exist, the script will prompt you to enter the directory path, and it will be saved for future use.

## Troubleshooting

- Ensure that `Node.js`, `npm`, and `screen` are installed on your system.
