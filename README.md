The name is a contraction of "[res]erved IPs". Yeah, I suck at names...

It's just a simple test to see if a given IP is in a reserved block (see:
https://en.wikipedia.org/wiki/Reserved\_IP\_addresses)

# Usage

Should be stupidly simple.

```go
package main

import (
    "net"

    "github.com/lillesvin/resips"
)

func main() {
    ip := net.ParseIP("192.168.1.2")
    if resips.IsReserved(ip) {
        // It's in a reserved block.
            // It's in a reserved block.
    }
}
```

