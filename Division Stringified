/***************************************************************************************
*                                                                                      *
*                  CODERBYTE BEGINNER CHALLENGE                                        *
*                                                                                      *
*  Division Stringified                                                                *
*  Using the JavaScript language, have the function DivisionStringified(num1,num2)     *
*  take both parameters being passed, divide num1 by num2, and return the result as    *
*  a string with properly formatted commas. If an answer is only 3 digits long,        *
*  return the number with no commas (ie. 2 / 3 should output "1"). For example:        *
*  if num1 is 123456789 and num2 is 10000 the output should be "12,345".               *
*                                                                                      *
*  SOLUTION                                                                            *
*  The first step is to divide the two number and get a whole number that you can      *
*  format according to the directions. I use RegExp to format the number.              *
*                                                                                      *
*  Steps for solution                                                                  *
*    1) Divide num1 by num2 and round to whole number                                  *
*    2) Use RegExp to format string as required                                        *
*                                                                                      *
***************************************************************************************/
function DivisionStringified(num1,num2) { 
 
  var tot = Math.round(num1 / num2);
  var newNum = tot.toString().replace(/(\d)(?=(\d{3})+(?!\d))/g, "$1,");

  return newNum;
         
}
