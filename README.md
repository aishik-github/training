# training

package main

import "fmt"
<!-- Start  from here -->
func fib() func() int {
	a, b := 0, 1
	return func() int {
		a, b = b, a+b
		return a
	}
}

func main() {
	f := fib()
	
	fmt.Println(f(), f(), f(), f(), f())
}


package main

import ("fmt")

func main(){
 fmt.Println("Hello World")

}
