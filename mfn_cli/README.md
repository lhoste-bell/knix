<!--
   Copyright 2020 The KNIX Authors

   Licensed under the Apache License, Version 2.0 (the "License");
   you may not use this file except in compliance with the License.
   You may obtain a copy of the License at

       http://www.apache.org/licenses/LICENSE-2.0

   Unless required by applicable law or agreed to in writing, software
   distributed under the License is distributed on an "AS IS" BASIS,
   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
   See the License for the specific language governing permissions and
   limitations under the License.
-->
# KNIX MicroFunctions Command Line Interface (CLI)

The package provides the `mfn` command based on the [KNIX MicroFunctions SDK](https://github.com/knix-microfunctions/knix/tree/master/mfn_sdk/).

The latest version of the CLI can be obtained from [KNIX releases](https://github.com/knix-microfunctions/knix/releases/).
It's also hosted at PyPI and can be installed with the PyPA recommended tool for installing Python packages:
``` sh
pip3 install mfn_cli
```

## Using the cli

### mfn login

The login action is used to obtain a valid user token for all subsequent operations.
The token will be updated/stored in ~/.mfn/config.yaml

``` sh
mfn login [--url <url>] [--user <username>] [--password <password>]
```

``` sh
$ mfn login --url https://knix.io/mfn --user test@example.com
Logging into https://knix.io/mfn as user test@example.com
Please enter the password: ************
$
```
