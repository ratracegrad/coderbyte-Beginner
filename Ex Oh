/***************************************************************************************
*                                                                                      *
*                  CODERBYTE BEGINNER CHALLENGE                                        *
*                                                                                      *
*  Ex Oh                                                                               *
*  Using the JavaScript language, have the function ExOh(str) take the str parameter   *
*  being passed and return the string true if there is an equal number of x's and o's, *
*  otherwise return the string false. Only these two letters will be entered in the    *
*  string, no punctuation or numbers. For example: if str is "xooxxxxooxo" then the    *
*  output should return false because there are 6 x's and 5 o's.                       *
*                                                                                      *
*  SOLUTION                                                                            *
*  My solution accounts for the one outlier which is when the length of the string     *
*  is not even. Since the count of Xs and Os have to be equal then the only way for    *
*  this to happen is if the length of the string is an even number. I am going to      *
*  loop through the string and count every X. Then I am going to compare this count    *
*  to half the length of the string. If they are equal then you have equal number of   *
*  Xs and Os.                                                                          *
*                                                                                      *
*  Steps for solution                                                                  *
*    1) Handle outlier first by seeing if str length is odd                            *
*    2) Loop thru each letter and count the number of Xs                               *
*    3) Compare count to 1/2 length of str and if same then return true                *
*    4) Else return false                                                              * 
*                                                                                      *
***************************************************************************************/
function ExOh(str) { 

  if (str.length % 2 === 1) {
    return false;
  } 
  else {  
    var tot = 0;
    for (var i = 0; i < str.length; i++) {
      if (str[i] === "x") {
        tot++;
      }
    }
    
    if (tot === (str.length / 2)) {
      return true;
    }
    else {
      return false;
    }

  }
         
}
