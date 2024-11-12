# Quicksort Pivots

in the lectures I only briefly mentioned strategies for determining a good pivot
for quicksort. The implementation on the slides simply picks the leftmost
element in the part of the array that we consider as a pivot. I also mentioned a
few other ways of picking a good pivot, e.g. randomly.

Median-of-three is also a good way of picking a pivot -- inspect the first,
middle, and last elements of the part of the array under consideration and
choose the median value. Using the probabilities for picking a pivot in a
particular part of the array (in the same way as we did on slide 34), argue
whether this method is more or less (or equally) likely to pick a good pivot
compared to simply choosing the first element. Assume that all permutations are
equally likely, i.e. the input array is ordered randomly.

I used the lecture slides/video on sorting, quicksort to look at slide 34 to review the material and compare my answer.

I certify that I have listed all sources used to complete this exercise, including the use of any Large Language Models. All of the work is my own, except where stated otherwise. I am aware that plagiarism carries severe penalties and that if plagiarism is suspected, charges may be filed against me without prior notice.

Your answer must derive probabilities for choosing a good pivot and
quantitatively reason with them.

If we choose the median-of-three, we have a $1/3$ possibility of choosing a good pivot. We would have partition sizes going at a size
of at most $(2n)/3$. While 2n/3 is under the at most partition size of 3n/4, we will pick a good pivot every 3 tries, which is less than the every two tries.
This would effectively mean we would find a pivot less times averagely than choosing the first element, so this would be less likely to choose a good pivot.

Add your answer to this markdown file. [This
page](https://docs.github.com/en/get-started/writing-on-github/working-with-advanced-formatting/writing-mathematical-expressions)
might help with the notation for mathematical expressions.
