// NOTES? idk but its from boots.dev and my understanding

==> GO programming stucture
=> package main lets the Go compiler know that we want this code to compile and run as a standalone program, as opposed to being a library that's imported by other programs.
=> import "fmt" imports the fmt (formatting) package from the standard library. It allows us to use fmt.Println to print to the console.
=> func main() defines the main function, the entry point for a Go program.

==> Two types of error
=> Compilation errors. Occur when code is compiled. It's generally better to have compilation errors because they'll never accidentally make it into production.
=> Runtime errors. Occur when a program is running. These are generally worse because they can cause your program to crash or behave unexpectedly.

==> Something interesting
-> GO has complex type numbers beside int, uint and float, 
-> complex type number has two sizes, i.e complex64 and complex128

-> It also has a rune type, idk whats that

==> SPEEDD
=> Go is faster than interpreted langs like python,js,php but it is slightly slower than natively compliled langs like c,c++ or rust.
-> its speed is more equally compared to langs that compile in a VM like java and c#.
-> though it is slower than natively compliled langs, it *compiles faster than those langs(c,rust .etc).
--> the reason it is slower compared to c/rust is every program of GO has some extra piece of code that helps managing memory (go runtime: https://go.dev/doc/faq#runtime)
-> One of the purposes of the Go runtime is to clean up unused memory at runtime. It includes a garbage collector that automatically frees up memory that's no longer in use.
-> Go is garbage collected. (The garbage collector attempts to reclaim memory that was allocated by the program, but is no longer referenced; such memory is called garbage)
-> light in lightweight, halka
-> concurrent, preferred for concurrency, did i do a spelling mistake?

:= walrus btw
var noob declaration but := does not work outside of a func
 
-> As a general rule, Java programs use more memory than comparable Go programs. There are several reasons for this, but one of them is that Java uses a virtual machine to interpret bytecode at runtime and typically allocates more on the heap.
-> On the other hand, Rust and C programs use slightly less memory than Go programs because more control is given to the developer to optimize the memory usage of the program. The Go runtime just handles it for us automatically.

-> Go often ables to allocate more memory on stack than heap compared to a lang like java does, stack allocations are more efficient/faster/performant than heap?
-> in C,C++,rust devs need do manually define when to allocate and free memory.
-> java handles memory / collected garbage as it runs on JVM (executes bytecode) but due to this java tends to use more memory than c/cpp/rust/go(executes bin/machinecode), java > go > c/rust

-> constants can not be declared using := , they have to be declared using the `const` keyword

-> Constants must be known at compile time. They are usually declared with a static value:
However, constants can be computed as long as the computation can happen at compile time.

// i hope ill revisit this soon

