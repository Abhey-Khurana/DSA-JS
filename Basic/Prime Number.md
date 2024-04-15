# Prime Number
In this Problem, we accept an integer as input and determine whether it is prime or not..

A <b>brute force</b> approach is we will start a loop from 2 and go till number-1.

An <b>Optimal</b> Solution can be we can run the loop till √number.

### Explanation
The loop runs until √n because if a number n can be expressed as n=a×b (where a and b are factors of n), then at least one of these factors (either a or b) will be less than or equal to √n.

````js
function isPrime(number) {
 for(var i=2;i<=Math.sqrt(number);i++)
 {
    if(i%number == 0)
        return false;
 }
 return true;
}
isPrime(73);

````