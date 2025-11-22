quadA.go -----


package main

import (
	"os"
	"strconv"
	"github.com/01-edu/z01"
)

func QuadA(x, y int) {
	if x <= 0 || y <= 0 {
		return
	}
	for r := 1; r <= y; r++ {
		for c := 1; c <= x; c++ {
			var char rune
			isFirstRow := r == 1
			isLastRow := r == y
			isFirstCol := c == 1
			isLastCol := c == x

			if (isFirstRow || isLastRow) && (isFirstCol || isLastCol) {
				char = 'o'
			} else if isFirstRow || isLastRow {
				char = '-'
			} else if isFirstCol || isLastCol {
				char = '|'
			} else {
				char = ' '
			}
			z01.PrintRune(char)
		}
		z01.PrintRune('\n')
	}
}

func main() {
	if len(os.Args) != 3 {
		return
	}
	x, err1 := strconv.Atoi(os.Args[1])
	y, err2 := strconv.Atoi(os.Args[2])
	if err1 != nil || err2 != nil {
		return
	}
	QuadA(x, y)
}