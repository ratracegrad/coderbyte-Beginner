/***************************************************************************************
*                                                                                      *
*                  CODERBYTE BEGINNER CHALLENGE                                        *
*                                                                                      *
*  Palindrome                                                                          *
*  Using the JavaScript language, have the function Palindrome(str) take the str       *
*  parameter being passed and return the string true if the parameter is a palindrome, *
*  (the string is the same forward as it is backward) otherwise return the string      *
*  false. For example: "racecar" is also "racecar" backwards. Punctuation and numbers  *
*  will not be part of the string.                                                     *
*                                                                                      *
*  SOLUTION                                                                            *
*  I have two outliers. The first is to remove all spaces between words since it can   *
*  cause the reverse string to be wrong. The second is to convert string to lower case *
*  so that any capitalized words cause a false answer. I am going to first remove all  *
*  spaces from the string. Then I am going to convert a new string that converts the   *
*  modified str into an array and then reverses the contents and then converts it back *
*  to a string. I will compare the modified string and the newStr to see if they are   *
*  equal signifying I have a Palindrome.                                               *
*                                                                                      *
*  Steps for solution                                                                  *
*    1) Modify str by removing all spaces and converting to lower case.                *
*    2) Create a new string by converting modified str into an array, reverse it and   *
*       then convert it back to a string                                               *
*    3) Compare two strings to see if equal meaing I have a Palindrome                 *
*                                                                                      *
***************************************************************************************/

function Palindrome(str) { 

  str = str.replace(/ /g,"").toLowerCase();
  var compareStr = str.split("").reverse().join("");

  if (compareStr === str) {
    return true;
  } 
  else {
    return false;
  } 

}
