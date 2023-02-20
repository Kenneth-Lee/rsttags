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

   ```rsttags <dir_to_sphinx_source>```
