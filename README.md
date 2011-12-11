# ganglia chef cookbook

Installs/Configures ganglia

## Overview

Installs/Configures ganglia

## Attributes

* `[:ganglia][:home_dir]`             -  (default: "/var/lib/ganglia")
* `[:ganglia][:log_dir]`              -  (default: "/var/log/ganglia")
* `[:ganglia][:conf_dir]`             -  (default: "/etc/ganglia")
* `[:ganglia][:pid_dir]`              -  (default: "/var/run/ganglia")
* `[:ganglia][:data_dir]`             -  (default: "/var/lib/ganglia/rrds")
* `[:ganglia][:user]`                 -  (default: "ganglia")
* `[:ganglia][:send_port]`            -  (default: "8649")
* `[:ganglia][:rcv_port]`             -  (default: "8649")
* `[:ganglia][:monitor][:run_state]`  -  (default: "start")
* `[:ganglia][:server][:run_state]`   -  (default: "start")
* `[:users][:ganglia][:uid]`          -  (default: "320")
* `[:groups][:ganglia][:gid]`         -  (default: "320")

## Recipes 

* `default`                  - Base configuration for ganglia
* `monitor`                  - Ganglia monitor -- discovers and sends to its ganglia_server
* `server`                   - Ganglia server -- contact point for all ganglia_monitors
## Integration

Supports platforms: debian and ubuntu

Cookbook dependencies:
* java
* runit
* metachef


## License and Author

Author::                Chris Howe - Infochimps, Inc (<coders@infochimps.com>)
Copyright::             2011, Chris Howe - Infochimps, Inc

Licensed under the Apache License, Version 2.0 (the "License");
you may not use this file except in compliance with the License.
You may obtain a copy of the License at

    http://www.apache.org/licenses/LICENSE-2.0

Unless required by applicable law or agreed to in writing, software
distributed under the License is distributed on an "AS IS" BASIS,
WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
See the License for the specific language governing permissions and
limitations under the License.

> readme generated by [cluster_chef](http://github.com/infochimps/cluster_chef)'s cookbook_munger
