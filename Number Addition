/***************************************************************************************
*                                                                                      *
*                  CODERBYTE BEGINNER CHALLENGE                                        *
*                                                                                      *
*  Number Addition                                                                     *
*  Using the JavaScript language, have the function NumberSearch(str) take the str     *
*  parameter, search for all the numbers in the string, add them together, then        *
*  return that final number. For example: if str is "88Hello 3World!" the output       *
*  should be 91. You will have to differentiate between single digit numbers and       *
*  multiple digit numbers like in the example above. So "55Hello" and "5Hello 5"       *
*  should return two different answers. Each string will contain at least one letter   *
*  or symbol.                                                                          *
*                                                                                      *
*  SOLUTION                                                                            *
*  I only want numbers in the string so I am using RegExp to remove everything that    *
*  is not a number. Then convert that to an array. Loop thru each number in the array  *
*  and add tot to get the answer.                                                      *
*                                                                                      *
*  Steps for solution                                                                  *
*    1) Initialize tot to zero                                                         *
*    2) Remove everything but numbers from string and convert to array                 *
*    3) Loop thru each number in array and add to tot                                  *
*    4) Return tot for answer                                                          *
*                                                                                      *
***************************************************************************************/

function NumberAddition(str) { 

    var tot = 0;
    
    str = str.replace(/[^0-9\.]+/g," ").split(" ");
    for (var i = 0; i < str.length; i++) {
        tot += Number(str[i]);
    }
  
  return tot;
         
}
