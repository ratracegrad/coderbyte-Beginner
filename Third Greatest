/***************************************************************************************
*                                                                                      *
*                  CODERBYTE BEGINNER CHALLENGE                                        *
*                                                                                      *
*  Third Greatest                                                                      *
*  Using the JavaScript language, have the function ThirdGreatest(strArr) take the     *
*  array of strings stored in strArr and return the third largest word within in.      *
*  So for example: if strArr is ["hello", "world", "before", "all"] your output should *
*  be world because "before" is 6 letters long, and "hello" and "world" are both 5,    *
*  but the output should be world because it appeared as the last 5 letter word in     *
*  the array. If strArr was ["hello", "world", "after", "all"] the output should be    *
*  after because the first three words are all 5 letters long, so return the last one. *
*  The array will have at least three strings and each string will only contain        *
*  letters.                                                                            *
*                                                                                      *
*  SOLUTION                                                                            *
*  I am going to sort the array in descending order using the length of each entry.    *
*  Once sorted the third greatest number is in array position 2.                       *
*                                                                                      *
*  Steps for solution                                                                  *
*    1) Sort array in decending order based on length of entry                         *
*    2) Return the entry in the 3rd spot                                               *
*                                                                                      *
***************************************************************************************/

function ThirdGreatest(strArr) { 

  strArr.sort(function(a, b){
      return b.length - a.length; 
    });
    
   return strArr[2];
         
}
