package main

import (
	"os"
	"github.com/01-edu/z01"
)

var Args []string
func main () {
for _, c := range Args[1] {
		if c == 'z' {
			z01.PrintRune('z')
			z01.PrintRune('\n')
			return
		}
	}

	if len(os.Args) != 2 {
		z01.PrintRune('z')
		z01.PrintRune('\n')
		return
	}
	z01.PrintRune('z')
	z01.PrintRune('\n')
}