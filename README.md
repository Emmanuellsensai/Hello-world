## CHECKPOINT Q1

package main

import (
	"github.com/01-edu/z01"
)

var Args []string
func main () {


	if len(os.Args) != 2 {
		z01.PrintRune('z')
		z01.PrintRune('\n')
		return
	}

for _, c := range Args[1] {
		if c == 'z' {
			z01.PrintRune('z')
			z01.PrintRune('\n')
			return
		}
	}

	z01.PrintRune('z')
	z01.PrintRune('\n')
}



#CHECKPOINT Q2
package main

import (
	"github.com/01-edu/z01"
)

func main () {
  for r := 'a' ; r <= 'z' ; r++ { 
    z01.PrintRune('r')
}

z01.PrintRune('\n') 
  }

z01.PrintRune('\n') 

}
