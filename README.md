# phylum-js-submit

Utility script to submit package-lock.json and yarn.lock files to the Phylum API

## Prerequisites
* NodeJS
* NPM
* Phylum-cli

## Installation
1. Install prerequisite software
2. Clone this repository
```sh
git clone https://github.com/peterjmorgan/phylum-js-submit.git
```
3. Change to the phylum-js-submit directory
```sh
cd phylum-js-submit
```
4. Install NodeJS dependencies via NPM
```sh
npm install
```
5. Optionally, install globally so phylum-js-submit is set up in NPM's path
```sh
npm install -g
```

## Usage
```
$ node phylum-js-submit.js -h
Options:
      --version     Show version number                                [boolean]
  -t, --type        Type of file to process (`package` or `yarn`, defaults to
                    `package`)                                          [string]
  -H, --heuristics  Submit previously processed packages for heuristics only,
                    not a full processing run                          [boolean]
  -d, --dry-run     Print the list of packages that would be submitted, but do
                    not actually submit them                           [boolean]
  -h, --help        Show help                                          [boolean]
```
Submit a package-lock.json textfile to Phylum API
```sh
phylum-js-submit.js -t package <path_to_package-lock.json>
```

Submit a yarn.lock textfile to Phylum API
```sh
phylum-js-submit.js -t yarn <path_to_yarn.lock>
```
