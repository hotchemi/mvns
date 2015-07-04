mvns [![PyPI version](https://badge.fury.io/py/mvns.svg)](http://badge.fury.io/py/mvns)
====

CLI tool to search library in maven central repository.

Install
-------

Use `pip` or `easy_install`.

```sh
pip install mvns
```

or

```sh
easy_install mvns
```

Usage
-----

### Search by query

```sh
> mvns picasso
compile 'com.squareup.picasso:picasso:2.5.2'
compile 'com.squareup.picasso:picasso-parent:2.5.2'
compile 'it.sephiroth.android.library.picasso:picasso-sample:2.1.6'
compile 'com.squareup.picasso:picasso-sample:2.5.2'
compile 'com.squareup.picasso:picasso-pollexor:2.5.2'
compile 'com.twotoasters.servos:util-picasso:1.0.0'
compile 'com.marvinlabs:android-slideshow-widget-picasso-plugin:0.5.0'
```

### Search by groupId and so on

- `-g` Specify groupId.
- `-a` Specify artifactId.
- `-v` Specify version.

```sh
mvns -g com.squareup.picasso -a picasso -v 2.5.2
compile 'com.squareup.picasso:picasso-parent:2.5.2'
```

### Select all version

- `-A` Show all version.

```sh
mvns -g com.squareup.picasso -a picasso -A
compile 'com.squareup.picasso:picasso:2.3.4'
compile 'com.squareup.picasso:picasso:2.3.3'
compile 'com.squareup.picasso:picasso:2.3.2'
compile 'com.squareup.picasso:picasso:2.3.1'
compile 'com.squareup.picasso:picasso:2.3.0'
```

### Limit number of result.

- `-m` Limit number of result. default is 20.

```sh
mvns picasso -m 1
compile 'com.squareup.picasso:picasso:2.3.4'
```

Support
-------

Supports Python 2.7 and 3.4.

Contribute
----------

1. Fork it
2. Create your feature branch (`git checkout -b my-new-feature`)
3. Commit your changes (`git commit -am 'Added some feature'`)
4. Push to the branch (`git push origin my-new-feature`)
5. Create new Pull Request

ChangeLog
---------

- 2015/07/05 0.1.3 release.
- 2015/05/11 0.1.2 release.
- 2014/09/20 0.1.1 release.
- 2014/09/14 0.1.0 release.

Licence
-------

```
 Copyright 2015 Shintaro Katafuchi

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
