# Hello-world
This repository is for practicing the GitHub Flow.
I'm aiming to be a skilled Data Engineer



interviewn=`grep -H "licen" interviews/* |grep "\"" | cut -f1 -d ":" | rev | cut -f1 -d "-" | rev`
interview="cat interviews/interview-$interviewn"
export interviewnum=$interviewn
echo $interviewnum
$interview
echo $MAIN_SUSPECT