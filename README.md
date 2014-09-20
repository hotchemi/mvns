mvns
====

[![Downloads](https://pypip.in/v/mvns/badge.png)](https://pypi.python.org/pypi/mvns/)

CLI tool to search library in maven central repository.

Install
-------

Use `pip` or `easy_install`.

```sh
pip install mvns
```

or

```sh
easy_install install mvns
```

Usage
-----

### Search by query

```sh
> mvns picasso
com.squareup.picasso:picasso:2.3.4
it.sephiroth.android.library.picasso:picasso:2.3.4.3
com.squareup.picasso:picasso-parent:2.3.4
it.sephiroth.android.library.picasso:picasso-sample:2.1.6
com.squareup.picasso:picasso-sample:2.3.4
com.squareup.picasso:picasso-pollexor:2.3.4
com.marvinlabs:android-slideshow-widget-picasso-plugin:0.5.0
```

### Search by groupId and so on

- `-g` Specify groupId.
- `-a` Specify artifactId.
- `-v` Specify version.

```sh
mvns -g com.squareup.picasso -a picasso -v 2.3.4
com.squareup.picasso:picasso:2.3.4
```

### Select all version

- `-A` Show all version.

```sh
mvns -g com.squareup.picasso -a picasso -A
com.squareup.picasso:picasso:2.3.4
com.squareup.picasso:picasso:2.3.3
com.squareup.picasso:picasso:2.3.2
com.squareup.picasso:picasso:2.3.1
com.squareup.picasso:picasso:2.3.0
com.squareup.picasso:picasso:2.2.0
com.squareup.picasso:picasso:2.1.1
com.squareup.picasso:picasso:2.1.0
com.squareup.picasso:picasso:2.0.2
com.squareup.picasso:picasso:2.0.1
```

### Limit number of result.

- `-m` Limit number of result. default is 20.

```sh
mvns picasso -m 1
com.squareup.picasso:picasso:2.3.4
```

Support
-------

Python 2.7 and 3.4 are supported.

Contribute
----------

1. Fork it
2. Create your feature branch (`git checkout -b my-new-feature`)
3. Commit your changes (`git commit -am 'Added some feature'`)
4. Push to the branch (`git push origin my-new-feature`)
5. Create new Pull Request

ChangeLog
---------

- 2014/09/20 0.1.1 release.
- 2014/09/14 0.1.0 release.

Licence
-------

```
 Copyright 2014 Shintaro Katafuchi

 Licensed under the Apache License, Version 2.0 (the "License");
 you may not use this file except in compliance with the License.
 You may obtain a copy of the License at

 http://www.apache.org/licenses/LICENSE-2.0

 Unless required by applicable law or agreed to in writing, software
 distributed under the License is distributed on an "AS IS" BASIS,
 WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 See the License for the specific language governing permissions and
 limitations under the License.
```
