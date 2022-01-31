# Clean Ubuntu Install

[![The MIT License](https://img.shields.io/badge/license-MIT-E95420?style=flat)](LICENSE)

Install and setup scripts for fresh install

## Install

Clone the repo

```text
git clone https://github.com/trevor-moon/install-programs.git
```

Move into the clone directory

```text
cd install-programs
```

Make sure package manager folder contents are executable

## Notes

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
