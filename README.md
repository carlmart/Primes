# Prime number generator

##  R> source("Primes.R")
### usage: primes(13)

     // R Language function primes()
     primes = function(n) {
           if (n >= 2) {
               s = seq(2,n)
               p = c()
               for (i in seq(2,n)) {
                 if(any(s==i)){
                  p = c(p,i)
                  s = c(s[(s%%i) != 0],i )
               }} 
           return (p) }
          else {
               stop("Input at least 2")
           }
         }



