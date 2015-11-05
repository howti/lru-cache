lru-cache
=========
LRU cache implemented in golang

Usage
=====
```go
package main
import(
    "github.com/howti/lru-cache"
)
func main() {
	lru := New(0)
	lru.Add("Testkey", 1234)
	val, ok := lru.Get("Testkey")
    fmt.Println("Is cache hit?", ok, "Value:", val)
}
```