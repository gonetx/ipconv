# gonetx/ipconv
<p align="center">
  <a href="https://pkg.go.dev/github.com/gonetx/ipconv">
    <img src="https://img.shields.io/badge/%F0%9F%93%9A%20godoc-pkg-00ACD7.svg?color=00ACD7&style=flat">
  </a>
  <a href="https://goreportcard.com/report/github.com/gonetx/ipconv">
    <img src="https://img.shields.io/badge/%F0%9F%93%9D%20goreport-A%2B-75C46B">
  </a>
  <a href="https://codecov.io/gh/gonetx/ipconv">
    <img src="https://codecov.io/gh/gonetx/ipconv/branch/main/graph/badge.svg?token=05UN78X11O"/>
  </a>
  <a href="https://github.com/gonetx/ipconv/actions?query=workflow%3ASecurity">
    <img src="https://img.shields.io/github/workflow/status/gonetx/ipconv/Security?label=%F0%9F%94%91%20gosec&style=flat&color=75C46B">
  </a>
  <a href="https://github.com/gonetx/ipconv/actions?query=workflow%3ATest">
    <img src="https://img.shields.io/github/workflow/status/gonetx/ipconv/Test?label=%F0%9F%A7%AA%20tests&style=flat&color=75C46B">
  </a>
  <a>
    <img src="https://counter.gofiber.io/badge/gonetx/ipconv">
  </a>
</p>

`ipconv` is a package providing utility functions to convert ip with high performance.

# Benchmark
Here is the benchmark with `2.4 GHz 8-Core Intel Core i9`:
```hs
$ GOMAXPROCS=1 go test -bench='Ipconv' -benchmem -benchtime=10s 
Benchmark_Ipconv_V42Long        604734988               18.5 ns/op             0 B/op          0 allocs/op
Benchmark_Ipconv_Long2V4        803246886               15.0 ns/op             0 B/op          0 allocs/op
```
