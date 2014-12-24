/***************************************************************************************
*                                                                                      *
*                  CODERBYTE BEGINNER CHALLENGE                                        *
*                                                                                      *
*  Powers of Two                                                                       *
*  Using the JavaScript language, have the function PowersofTwo(num) take the num      *
*  parameter being passed which will be an integer and return the string true if       *
*  it's a power of two. If it's not return the string false. For example if the        *
*  input is 16 then your program should return the string true but if the input is     *
*  22 then the output should be the string false                                       *
*                                                                                      *
*  SOLUTION                                                                            *
*  To find if a number is a power of 2 you divide number by 2 repeatedly.              *
*  If final number is a two then it is a power of 2. I will use a while loop to        *
*  handle the repeated division by two. I will use modulus to determine if final       *
*  number is two meaning we have a number that is a power of 2.                        *
*                                                                                      *
*  Steps for solution                                                                  *
*    1) Initialize vars divis and newNum                                               *
*    2) Loop by dividing number by 2 and seeing if it is an even number                *
*    3) Test if last number is 2 meaning it is a power of 2                            *
*                                                                                      *
***************************************************************************************/
function PowersofTwo(num) { 

  var divis;
  var newNum;
  
  divis = num % 2;
  newNum = num / 2;
  while ( divis === 0 && newNum !== 2) {
    divis = newNum % 2;
    newNum = newNum / 2;
  }

  if (newNum === 2) {
    return true;
  }
  else {
    return false;
  }
}
