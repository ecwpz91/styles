# Styles

Bootstrap toolkit that embeds Font Awesome for developing with HTML, CSS, and JS.

# Getting Started

To use this project, you'll need (at minimum):

- Node.js' package ecosystem, [npm][1]

## Install

### GNU/Linux, or macOS

```sh
#!/bin/bash

GITUSER="ecwpz91"
git clone https://github.com/${GITUSER}/styles.git
cd styles
```

### No `git`? No problem!

```sh
#!/bin/bash

DIRPATH="${HOME}/Downloads/styles"; GITUSER="ecwpz91"; RELEASE="master"
GITREPO="https://github.com/${GITUSER}/styles/archive/${RELEASE}.zip"
ARCHIVE="$(printf "%s" "${GITREPO##*/}")"

# Download and extract
wget ${GITREPO} \
&& temp="$(mktemp -d)" \
&& unzip -d $temp ${ARCHIVE} \
&& mkdir -p ${DIRPATH} \
&& mv $temp/*/* ${DIRPATH} \
&& rm -rf $temp ${ARCHIVE} \
&& cd ${DIRPATH} \
&& unset DIRPATH GITUSER GITREPO ARCHIVE
```

## Setup

### Using `npm`

```sh
cd styles/
npm i
```

# Usage

### Let's build it!

```sh
grunt
```

#### What does this script do?

It compiles Bootstrap CSS and JS, as well as, Font Awesome iconography into `dist`.


[1]: https://www.npmjs.com/
