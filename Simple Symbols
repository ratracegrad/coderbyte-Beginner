/***************************************************************************************
*                                                                                      *
*                  CODERBYTE BEGINNER CHALLENGE                                        *
*                                                                                      *
*  Simple Symbols                                                                      *
*  Using the JavaScript language, have the function SimpleSymbols(str) take the str    *
*  parameter being passed and determine if it is an acceptable sequence by either      *
*  returning the string true or false. The str parameter will be composed of + and =   *
*  symbols with several letters between them (ie. ++d+===+c++==a) and for the string   *
*  to be true each letter must be surrounded by a + symbol. So the string to the left  *
*  would be false. The string will not be empty and will have at least one letter.     *                                                 *
*                                                                                      *
*  SOLUTION                                                                            *
*  When reading the directions for this challenge you have to be aware of the adage    *
*  "Attention to detail, all the time!" The instructions immediately tell you that     *
*  you will have two outliers that you have to account for in your solution. They are  *
*  the first and last characters. If these are letters then you have to return false   *
*  because there cannot be a + before or after these letters.
*                                                                                      *
*  Steps for solution                                                                  *
*    1) Convert string to an Array.                                                    *
*    2) Loop thru each letter in array                                                 *
*    3) If first character or last character is letter a-z then return false  (outlier)*
*    4) If charcter is string then check if letter before and after is + and if not    *
*       then return false                                                              *
*    5) If looped through whole array and everything matches then return true          *
*                                                                                      *
***************************************************************************************/

function SimpleSymbols(str) { 

  var arr = str.toLowerCase().split("");
  for (var i = 0; i < arr.length; i++) {
    if (arr[i] >= "a" && arr[i] <= "z") {
      if (i === 0 || i === arr.length) {
        return false;
      }
      
      if (arr[i-1] !== "+" || arr[i+1] !== "+") {
        return false;
      }
    }
  }
  
  return true; 
         
}
