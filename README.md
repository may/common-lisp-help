# common-lisp-help
Yet another common lisp cheat sheet, not comprehensive, biased towards what I need.

## license

Copyright 2022-2023 Nicholas E. May

This file is part of common-lisp-help.

```
;; common-lisp-help is free software: you can redistribute it and/or modify it
;; under the terms of the GNU General Public License as published
;; by the Free Software Foundation, either version 3 of the License, or
;; (at your option) any later version.
;;
;; common-lisp-help is distributed in the hope that it will be useful, but
;; WITHOUT ANY WARRANTY; without even the implied warranty of
;; MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.
;;
;; See the GNU General Public License for more details.
;;
;; You should have received a copy of the GNU General Public License
;; along with common-lisp-help. If not, see <https://www.gnu.org/licenses/>.
```

# benchmarking/timing

`(time (hello))`

# debugging & learning

## `describe`

- `(describe *standard-output*)`
- `(describe #'defun)`
etc.

<img width="1407" alt="image" src="https://user-images.githubusercontent.com/82888/204191127-35d4b443-1738-4b2c-a4d1-da4b6d4a2a36.png">


# executable

On SBCL:

```lisp
(defun hello ()
  (print "hello"))

(sb-ext:save-lisp-and-die #P"~/hello.exe" :toplevel #'hello :executable t)
```
