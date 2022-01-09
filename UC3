echo "head="$countHead
echo "tail="$countTail

noOfCounts[tail]=$countTail
noOfCounts[head]=$countHead

echo ${noOfCounts[@]}



function wining(){

array=($(for size in ${noOfCounts[@]}
do
echo $size
done | sort ))
echo "sorted value"
echo ${array[@]}
lastindex=$((${#array[@]}-1))

MaxWin=${array[$lastindex]}
for i in ${!noOfCounts[@]}
do
 if [ ${noOfCounts[$i]} -eq $MaxWin ]
 then
     echo "maximum times win= "$i
   fi
done
}

wining
