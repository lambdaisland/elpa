**lambdaisland/elpa IS NOT ACCEPTING PACKAGES AT THIS POINT**

To add a package here, or to set up your own ELPA repo, do this

``` emacs-lisp
(require 'package-x)

(setq package-archive-upload-base "~/your/own/elpa")
```

Now run `M-x package-upload-file`, and select the package you want to add to
your local ELPA repo. This can be a single `.el` file, or a tarball created with
Cask.

This will copy over the package, and update `archive-contents`. Now you can
commit and push.
