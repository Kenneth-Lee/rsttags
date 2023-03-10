# rsttags

## Introduction

This is a tags generator for python sphinx tool to generate tags from index
role or directive.

Dtag role is also supported. dtag is a sphinx extension written by me to
generate tag for the set set of rst documents. See misc/dtags.py for detail.

New requirements are welcomed.

## Usage

1. Make sure python3 is in /usr/bin (or you can change the header of rsttag file).
2. copy the rsttags file to the the path that you can run it. (such as ~/bin or
   /usr/local/bin)
3. run the follow command in the directory you want to generate tags file:
   `rsttags`. you can specific 0 or more directory or rst file as input. If no
   direcory is specific, current directory is used.

There some tag types are used. They are:

```
i: index (match :index:`xxx` or .. index:: xxx)
d: doc (match :doc:`xxx`)
D: dtag (match :dtag:`xxx`)
f: filename
l: link (match .. _`xxx`: or .. _xxx:)
r: reference (match :ref:`xxx`)
s: section name
```

These are supported options:
```
  -t
  --type-before-name
      Add type prefixes to tag names. So a section xxx will
      become s_xxx. default is "idDflrs".
  
  -T
  --types
     Set tags types. Default is "idDflrs".
```
