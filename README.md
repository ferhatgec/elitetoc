# [elite](https://github.com/ferhatgec/elite)toc
## [elite](https://github.com/ferhatgec/elite) -> c converter

### input:
```rs
required_version is 0.1

set ProjectName as "elitetopy"
set HOME        as env "HOME"


for argument "install" [
    use exec "cargo install --path ."

    for exists "{HOME}.cargo/bin/{ProjectName}" [
        println "{ProjectName} installed to {HOME}.cargo/bin/{ProjectName}."
    ]

    use signal "exit"
]
```

### output
```c
#include <stdio.h> 
#include <string.h> 
#include <sys/stat.h> 
#include <stdbool.h> 
#include <stdlib.h>

// exists(), get_os() and get_arch() here.

int main(int argc, char** argv) {
if("0.1" != "0.1")
{
 printf("elite: Required higher version\n");
 return 1;
}
char* ProjectName = "elitetoc";
char* HOME = "/home/gech";
if(argc >= 2 && strcmp(argv[argc - 1], "install") == 0)
{
 system("cargo install --path .");
 if(exists("/home/gech/.cargo/bin/elitetoc"))
{
  printf("elitetoc installed to /home/gech/.cargo/bin/elitetoc.\n");
}
 return 1;
}
}

```

### elitetoc licensed under the terms of MIT License
