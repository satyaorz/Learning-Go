==> GO programming stucture

=> package main lets the Go compiler know that we want this code to compile and run as a standalone program, as opposed to being a library that's imported by other programs.
=> import "fmt" imports the fmt (formatting) package from the standard library. It allows us to use fmt.Println to print to the console.
=> func main() defines the main function, the entry point for a Go program.

==> Two types of error
=> Compilation errors. Occur when code is compiled. It's generally better to have compilation errors because they'll never accidentally make it into production.
=> Runtime errors. Occur when a program is running. These are generally worse because they can cause your program to crash or behave unexpectedly.
