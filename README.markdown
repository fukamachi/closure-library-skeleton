# Skeleton for Google Closure Library

## Quick Start

1. Download Closure Library

    svn co http://closure-library.googlecode.com/svn/trunk/ closure-library

2. Resolve dependencies

    python closure-library/closure/bin/build/depswriter.py --root_with_prefix="scripts ../../../scripts" --output_file=deps.js

'deps.js' will be created.

3. Open

    open index.html

## with Compiler

1. Download Closure Compiler

    wget http://closure-compiler.googlecode.com/files/compiler-latest.zip
    unzip compiler-latest.zip

Be sure 'compiler.jar' is in the project root.

2. Compile

    python closure-library/closure/bin/build/closurebuilder.py \
      -c compiler.jar -f "--compilation_level=ADVANCED_OPTIMIZATIONS" \
      -n skel.App -o compiled --output_file=files/skel.js \
      --root=closure-library --root=scripts \

Look 'files/skel.js'.

