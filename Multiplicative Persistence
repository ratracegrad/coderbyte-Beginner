/***************************************************************************************
*                                                                                      *
*                  CODERBYTE BEGINNER CHALLENGE                                        *
*                                                                                      *
*  Multiplicative Persistence                                                          *
*  Using the JavaScript language, have the function FirstFactorial(num) take the num   *
*  parameter being passed and return the factorial of it (ie. if num = 4,              *
*  return (4 * 3 * 2 * 1)). For the test cases, the range will be between 1 and 18.    *                                                     *
*                                                                                      *
*  SOLUTION                                                                            *
* The challenge passes a string but it expects us to do Math on it so it needs to      *
*  be converted to numbers. I will use the base 10 parameter of the toString()         *
*  function to convert each entry in the array to a Number. Then I am going to         *
*  multiply each entry in the array to get a total. I will repeat this until my        *
*  total is a single digit number. The number of times I multiplied is returned        *
*  as the answer.                                                                      *
*                                                                                      *
*  Steps for solution                                                                  *
*    1) Initialize vars sum and loop                                                   *
*    2) Convert str to an array of numbers                                             *
*    3) Loop until the sum of digits in array is a single digit number                 *
*    4) Return number of loops as answer                                               *
*                                                                                      *
***************************************************************************************/

function MultiplicativePersistence(num) { 

   var sum, loop = 0;
    var val1 = num.toString(10).split("");
    
     while( val1.length > 1 ) {
        sum = 1;
        val1.forEach( function(number) {
            sum = sum * number;
        });
        val1 = sum.toString(10).split("");
        loop++;
    } ;
    
    return loop;
         
}
