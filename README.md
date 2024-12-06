# exam-shell-apache-cgi

Empty repo for exam purposes

This repo is configured for executing bash and cgi scripts.

You can create bash scripts in the top level working directory and
execute those scripts via the path 

```
http://localhost/cgi-bin/{SCRIPT_NAME}
```

For example, if you have a file called *test.sh* in the current working directory 
with the following content with executable permission:

```bash
#!/bin/bash

echo "Content-type: text/plain"
echo
echo "Hello"
```

Then you can run the script via curl using the following:

```shell
$ curl localhost/cgi-bin/test.sh
```

