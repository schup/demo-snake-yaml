# Library Scanning Demo
Example for NexusIQ scanning for 3rd party libraries.

The observed licences for SnakeYaml (org.yaml:snakeyaml) is contains GPL whereas
the declared is Apache-2.0

SnakeYaml is used by SpringBoot to parse YAML config files and therefore widely used.

It is not clear how NexusIQ actually identifies observed licenses.

SnakeYaml contains a Base64 encoder which is multi-licensed.
https://github.com/asomov/snakeyaml/blob/master/src/main/java/org/yaml/snakeyaml/external/biz/base64Coder/Base64Coder.java

```
//
// This module is multi-licensed and may be used under the terms
// of any of the following licenses:
//
//  EPL, Eclipse Public License, V1.0 or later, http://www.eclipse.org/legal
//  LGPL, GNU Lesser General Public License, V2.1 or later, http://www.gnu.org/licenses/lgpl.html
//  GPL, GNU General Public License, V2 or later, http://www.gnu.org/licenses/gpl.html
//  AL, Apache License, V2.0 or later, http://www.apache.org/licenses
//  BSD, BSD License, http://www.opensource.org/licenses/bsd-license.php
//
// Please contact the author if you need another license.
// This module is provided "as is", without warranties of any kind.
```

