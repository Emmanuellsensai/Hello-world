<img width="761" height="496" alt="image" src="https://github.com/user-attachments/assets/63ecc109-5e58-4adf-8d99-e53e21d9dd6f" />



package piscine

import "github.com/01-edu/z01"

func PrintComb2() {
	for a := '0'; a <= '9'; a++ {
		for b := '0'; b <= '9'; b++ {
			for c := '0'; c <= '9'; c++ {
				for d := '0'; d <= '9'; d++ {
					if a >c || ( a == c  & b >= d ) {
						continue
					}

					z01.PrintRune(a)
					z01.PrintRune(b)
					z01.PrintRune(' ')
					z01.PrintRune(c)
					z01.PrintRune(d)

					if !(a == '9' && b == '8' && c == '9' && d == '9') {
						z01.PrintRune(',')
						z01.PrintRune(' ')
					}
				}
			}
		}
	}
	z01.PrintRune('\n')
}


## Mine
package piscine

import "github.com/01-edu/z01"

func PrintComb2() {
	for a := '0'; a <= '9'; a++ {
		for b := '0'; b <= '9'; b++ {
			for c := '0'; c <= '9'; c++ {
				for d := b + 1; d <= '9' || c > '0'; d++ {
					if d == ':' {
						continue
					}

					z01.PrintRune(a)
					z01.PrintRune(b)
					z01.PrintRune(' ')
					z01.PrintRune(c)
					z01.PrintRune(d)

					if !(a == '9' && b == '8' && c == '9' && d == '9') {
						z01.PrintRune(',')
						z01.PrintRune(' ')
					}
				}
			}
		}
	}
	z01.PrintRune('\n')
}





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
