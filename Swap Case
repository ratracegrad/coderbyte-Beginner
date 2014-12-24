/***************************************************************************************
*                                                                                      *
*                  CODERBYTE BEGINNER CHALLENGE                                        *
*                                                                                      *
*  Swap Case                                                                           *
*  Using the JavaScript language, have the function SwapCase(str) take the str         *
*  parameter and swap the case of each character. For example: if str is "Hello World" *
*  the output should be hELLO wORLD. Let numbers and symbols stay the way they are.    *                                                   *
*                                                                                      *
*  SOLUTION                                                                            *
*  I am going to be using a new string to store my modified results. I am going to     *
*  loop thru every character and covert it to UpperCase. Then I am going to compare    *
*  that to the character in the string. If they are the same - meaning both are        *
*  uppercase then I am going to return the lowercase of the character. If they are not *
*  the same then return the Uppercase character.
*                                                                                      *
*  Steps for solution                                                                  *
*    1) Create new string to hold my results                                           *
*    2) Loop thru each character in the string                                         *
*    3) Save the uppercase of this character in u                                      *
*    4) Compare uppercase to current character                                         *
*    5) If they are the same then return the lowercase                                 *
*    6) Else return uppercase                                                          *
*                                                                                      *
***************************************************************************************/

function SwapCase(str) { 

  var result = '';

  for (var i = 0; i < str.length; i++) {
    var c = str[i];
    var u = c.toUpperCase();

    result += u === c ? c.toLowerCase() : u;
  }

  return result;
         
}
