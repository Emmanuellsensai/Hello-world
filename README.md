<img width="1366" height="768" alt="image" src="https://github.com/user-attachments/assets/c1c52b98-d150-49fc-832f-4bee1a1f76c5" />



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
