/***************************************************************************************
*                                                                                      *
*                  CODERBYTE BEGINNER CHALLENGE                                        *
*                                                                                      *
*  First Factorial                                                                     *
*  Using the JavaScript language, have the function FirstFactorial(num) take the num   *
*  parameter being passed and return the factorial of it (ie. if num = 4,              *
*  return (4 * 3 * 2 * 1)). For the test cases, the range will be between 1 and 18.    *                                                     *
*                                                                                      *
*  SOLUTION                                                                            *
*  You can either use an iterative or recursive function to solve this challenge.      *
*  I am going to use an interative function. I am going to start with a value of 1     *
*  for my total and then keep multiplying it by the next number until I reach num.     *
*                                                                                      *
*  This function needs to account for a possible outlier - One and Zero.               *
*  If num is 1 or 0 then the answer is 1. By setting tot to value of 1 at              *
*  initialization, then it guaranteees that 1 will be returned if num is ever 0 or 1.  *
*  Steps for solution                                                                  *
*    1) Set var tot to 1.                                                              *
*    2) Loop from 2 to num and multiple tot by num to get new tot.                     *
*    3) Return tot for answer.                                                         *
*                                                                                      *
***************************************************************************************/

function FirstFactorial(num) { 

  var tot = 1;
  for (var i = 2; i <= num; i++) {
    tot *= i;
  }
   
  return tot;
         
}
