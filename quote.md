> In languages with a garbage collector (GC), the GC keeps track and cleans up memory that isn’t being used anymore,
 and we don’t need to think about it. Without a GC, it’s our responsibility to identify when memory is no longer
 being used and call code to explicitly return it, just as we did to request it. Doing this correctly has historically
 been a difficult programming problem. If we forget, we’ll waste memory. If we do it too early, we’ll have an invalid
 variable. If we do it twice, that’s a bug too. We need to pair exactly one allocate with exactly one free. 

> Rust takes a different path: the memory is automatically returned once the variable that owns it goes out of scope.

― Steve Klabnik, The Rust Programming Language