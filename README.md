# Go Map Access Panic

This repository demonstrates a common error in Go: accessing a nil map.  Attempting to access an element of a nil map will cause a runtime panic.

## The Bug

The `bug.go` file contains a simple program that attempts to access an element of an uninitialized map.  This will result in a panic.

## The Solution

The `bugSolution.go` file shows the corrected code.  It includes a nil check to prevent the panic by verifying that the map exists before trying to access its elements.

## How to reproduce the bug

1. Clone this repository
2. Run `go run bug.go`
3. Observe the panic.

## How to fix the bug

1. Implement a nil check.
2. Run `go run bugSolution.go`
3. No panic!