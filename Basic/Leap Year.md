# Leap Year
The program takes a year as input and checks if it meets the criteria for a leap year based on the Gregorian calendar rules.

The issue here is that while we understand the general solution, we are unable to apply the two conditions logically.

### Explanation
The problem is divided into two categories of years: century years and non-century years. A first set of conditions applies to non-century years, while a second set of conditions applies to century years. If any of the conditions is met, the year in input is a leap year.

````js
function isLeapYear(year) {
  if((year%4==0)&& (year%100!=0) || (year%400==0))
{
    return true;
}
    return false;
}
isLeapYear(1700);

````