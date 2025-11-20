# Hello-world
This repository is for practicing the GitHub Flow.
I'm aiming to be a skilled Data Engineer


<img width="1194" height="720" alt="image" src="https://github.com/user-attachments/assets/d8a06951-9b50-48cb-8a28-63691c3d8998" />

interviewn=`grep -H "licen" interviews/* |grep "\"" | cut -f1 -d ":" | rev | cut -f1 -d "-" | rev`
interview="cat interviews/interview-$interviewn"
export interviewnum=$interviewn
echo $interviewnum
$interview
echo $MAIN_SUSPECT


package main

import (
	"os"
	"github.com/01-edu/z01"
)

func main () {
for _, c := range os.Args[1] {
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