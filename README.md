# go-diskstate

## example

1. 

```
go get gitlab.com/tingshuo/go-diskstate/
```
2. 

```
import "gitlab.com/tingshuo/go-diskstate/diskstate"

import "fmt"

// example
func main() {
	state := diskstate.DiskUsage("/")
	fmt.Printf("All=%dM, Free=%dM, Available=%dM, Used=%dM, Usage=%d%%",
		state.All/diskstate.MB, state.Free/diskstate.MB, state.Available/diskstate.MB, state.Used/diskstate.MB, 100*state.Used/state.All)
}
```

