# Skeleton for Google Closure Library

## Download Closure Library

    svn co http://closure-library.googlecode.com/svn/trunk/ closure-library

## Resolve dependencies

    python closure-library/closure/bin/build/depswriter.py --root_with_prefix="scripts ../../../scripts" --output_file=deps.js

## Start

    open index.html

