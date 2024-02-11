# liberty-max.aktivisda.earth

This repository contains the data for the Liberty Max's instance of Aktivisda.

## Installation

### Getting started

This repository cannot be used on its own as it requires Aktivisda.

You need to create a sub-directory `aktivisda-core` with aktivisda source code.
You can directly clone `aktivisda` into this subdirectory :

```bash
git clone git@framagit.org:aktivisda/liberty-max.git
cd liberty-max
git clone git@framagit.org:aktivisda/aktivisda.git aktivisda-core
```

Or you can create a symbolic link (useful if you manage many instances in your computer) :

```bash
git clone git@framagit.org:aktivisda/liberty-max.git
git clone git@framagit.org:aktivisda/aktivisda.git aktivisda-core
ln -s <path to aktivisda core> <path to liberty-max>/aktivisda-core
```

### Installation

You can execute `npm` commands in `liberty-max` directory:

```
npm install
```

will call `npm install` in `aktivisda-core` (nothing done in `liberty-max`)

```
npm run serve
```

It will copy the data from `liberty-max` to `aktivisda-core` and then start call `npm run serve` in `aktivisda-core`.

Aktivisda will be accessible at `localhost:8080`

## Contributing

It's recommended to modify this repository through Backtivisda
