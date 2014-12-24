/***************************************************************************************
*                                                                                      *
*                  CODERBYTE BEGINNER CHALLENGE                                        *
*                                                                                      *
*  Letter Changes                                                                      *
*  Using the JavaScript language, have the function LetterChanges(str) take the str    *
*  parameter being passed and modify it using the following algorithm. Replace every   *
*  letter in the string with the letter following it in the alphabet                   *
*  (ie. c becomes d, z becomes a). Then capitalize every vowel in this new string      *
*  (a, e, i, o, u) and finally return this modified string.                            *
*                                                                                      *
*  SOLUTION                                                                            *
*  You have to realize that the string passed in may contain items other than letters  *
*  of the alphabet. If you find a character that is not a-z then just pass it along    *
*  to the newStr as is without any modification.  I am going to compare each letter    *
*  in the string to the alphabet string. If the letter is found then I am going to     *
*  return the next letter in the string unless the letter is z and them I am going     *
*  to return a. When finished I am going to use a RegExp to replace all lower case     *
*  vowels with upper case.
*                                                                                      *
*  Steps for solution                                                                  *
*    1) Create alphabet string that contains all letters of the alphabet               *
*    2) Loop through each letter in the string                                         *
*    3) If letter is Z then return a                                                   *
*    4) If letter is not a-z then return letter as is to newStr                        *
*    5) If letter is a-z then return the next character in the alphabet string         *
*    6) Replace all vowels with upper case with a RegExp replace() function            *
*                                                                                      *
***************************************************************************************/

function LetterChanges(str) { 

  var alphabet = "abcdefghijklmnopqrstuvwxyz";
  var newStr = "";
  var loc;

  for (var i = 0; i < str.length; i++) {
    loc = alphabet.indexOf(str[i]);
    if (loc === 25) {
      newStr = newStr + "a";
    } else if (loc === -1) {
      newStr = newStr + str[i];
    } else {          
      newStr = newStr + alphabet[loc + 1];
    }
  }
  
  return newStr.replace(/[aeiou]/g, function(letter) {return letter.toUpperCase()});  
         
}
