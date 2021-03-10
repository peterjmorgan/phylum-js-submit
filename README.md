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

## Usage
Submit a package-lock.json textfile to Phylum API
```sh
phylum-js-submit.js -t package <path_to_package-lock.json>
```

Submit a yarn.lock textfile to Phylum API
```sh
phylum-js-submit.js -t yarn <path_to_yarn.lock>
```
