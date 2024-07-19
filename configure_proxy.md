Fish configs
para crear un alias en fish:
* ```alias proxyon="export http_proxy=http://local.host:port/ && export https_proxy=http://local.host:port/ && env {http,https}_proxy=http://local.host:port"```
* ```funcsave proxyon```
