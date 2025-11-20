<img width="1366" height="768" alt="image" src="https://github.com/user-attachments/assets/d07bd7a7-8275-4ba2-b15d-6fbb54722a31" />





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
