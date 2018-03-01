Github Label Template
------------------------
[![Build Status](https://travis-ci.org/xavierchow/github-label-template.svg?branch=master)](https://travis-ci.org/xavierchow/github-label-template)
[![npm](http://img.shields.io/npm/v/github-label-template.svg?maxAge=2592000)](https://www.npmjs.org/package/github-label-template)

## Intro


Will you be satisfied and stuck with the default labels in the GitHub repository?
The answer may probably be NO; you always need to add some new ones, customize the colors, etc. 
Finally, you will come to an excellent label template(or you might find someone from others), whenever you create a new repository, you might want to reuse the labels your favor, but still with copying manually?

No... This command line tool tries to help you manipulate your GitHub label template efficiently.

## Recommended template
Feel free to export the lables of this [repo](https://github.com/xavierchow/github-label-template/labels) as a template.
![](/assets/template.png)

## Prerequisite
Node.js 4.4 or later.

## Install
`npm install github-label-template`

## Usage
```

  Usage: ghlbl [options]

  Options:

    -h, --help               output usage information
    -V, --version            output the version number
    -o, --owner [owner]      repo owner
    -r, --repo [repo]        repo name
    -t, --token [token]      github token
    -e, --export [filename]  export the lables to json file [filename]
    -d, --del                delete all existed labels
    -i, --import [filename]  import the labels from json file [filename]


```
### Samples

* Export all labels
  * `ghlbl -o xavierchow -r github-label-template -t <github-token> -e out.json`


* Clear all existed labels
  * `ghlbl -o xavierchow -r github-label-template -t <github-token> -d`

* Import labels from json template
  * `ghlbl -o xavierchow -r github-label-template -t <github-token> -i tmpl.json`


## License
MIT
