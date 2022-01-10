# Clean Ubuntu Install

[![The MIT License](https://img.shields.io/badge/license-MIT-E95420?style=flat)](LICENSE)

Install and setup scripts for fresh Ubuntu-based install

## Install

Clone the repo

```text
git clone https://github.com/trevor-moon/clean-install-ubuntu.git
```

Move into the clone directory

```text
cd clean-install-ubuntu
```

Update files to have execute permission

```text
chmod 755 src/*
```

## Usage

Use the scripts individually

```text
# install visual studio code
./src/install_code
```

or together

```text
# install curl then github cli
./src/install_curl && ./src/install_gh
```

## Notes

All scripts use the `apt` package manager.

Each script executes `sudo apt update` before each installation and executes without confirmation (-y or --yes flag). The general implementation is

```text
sudo apt update
sudo apt install {name} -y
```

## Roadmap

- [ ] Create a `main` script to run all scripts sequentially
- [ ] Create configuration file to determine which script(s) to run in `main`

## License

[![The MIT License](https://img.shields.io/badge/license-MIT-E95420?style=flat)](LICENSE)
