# PSD from CLI
Convert to PNG and extract text from Photoshop files using the CLI

## Requirements

This tool has no native dependencies (no need for ImageMagick or even Photoshop) thanks to the great work done by the folks of PSD.js. Unfortunately, not all image modes and depths are supported yet.
You just need to have a recent version of NodeJS installed on your system.

## Install

`npm install -g psd-cli`

Usage

### Convert a single file
```shell 
psd path/to/my_psd_file.psd -c
```
Creates `path/to/my_psd_file.png`

### Extract text from a single file
```shell 
psd path/to/my_psd_file.psd -t
```
Creates `path/to/my_psd_file.txt`

### Preview a single file
```shell 
psd path/to/my_psd_file.psd -o
```

Still creates `path/to/my_psd_file.png`

### Multiple file handling
```shell 
psd *.psd -o
```
Creates PNG files and opens them in your default image preview software

### Help

Full usage available by typing `psd --help`

Source: [npm package psd-cli](https://www.npmjs.com/package/psd-cli)
