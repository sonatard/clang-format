clang-format.el
========

Clang-format emacs integration for use with C/Objective-C/C++.
https://llvm.org/svn/llvm-project/cfe/trunk/tools/clang-format/clang-format.el

## Update from original
### Add provide statement
Add support for requrire statement. Now available (require 'clang-format) on init.el.

### Avoid empty buffer when executing clang-format-xxx without clang-format-binary
If clang-format is not installed, print error message on mini buffer.


## Usage
init.el
```lisp
(require 'clang-format)
(global-set-key (kbd "C-c i") 'clang-format-region)
(global-set-key (kbd "C-c u") 'clang-format-buffer)
```
