/***************************************************************************************
*                                                                                      *
*                  CODERBYTE BEGINNER CHALLENGE                                        *
*                                                                                      *
*  Letter Count I                                                                      *
*  Have the function LetterCountI(str) take the str parameter being passed and return  *
*  the first word with the greatest number of repeated letters. For example:           *
*  "Today, is the greatest day ever!" should return greatest because it has 2 e's      *
*  (and 2 t's) and it comes before ever which also has 2 e's. If there are no words    *
*  with repeating letters return <b>-1</b>. Words will be separated by spaces.         *
                                                 *
*                                                                                      *
*  SOLUTION                                                                            *
*  The first step is to remove all punctuation from the string being passed in which   *
*  I do with the replace function. I also convert string to LowerCase to account for   *
*  any words in the string that might be ProperCase. I then convert string into an     *
*  array of words breaking on space. Next I loop through each word in the array.       *
*  I loop through each character in the word and count the number of times the letter  *
*  repeats. Then I compare the max times a letter is repeated in that word to the      *
*  current value of maxCt which is initalized with a value of 1. If the number of      *
*  repeated characters is greater then I update the maxCt with the new value and the   *
*  current word is the maxWord.  When finished loop I check to see if any word has     *
*  repeated characters and if not return -1 else return the word with max repeated     *
*  characters.                                                                         *
*                                                                                      *
*  Steps for solution                                                                  *
*    1) Initialize variables                                                           *
*    2) Convert string to lowerCase, remove all punctuation and store in array         *
*    3) Loop through each word in array and count the occurance of each letter         *
*    4) Compare occurance of repeated letter to maxCt                                  *
*    5) If greater update maxCt to new value and store word in maxWord                 *
*    6) Return word with max repeated characters or -1                                 *
*                                                                                      *
***************************************************************************************/

function LetterCountI(str) {
    var ctObj, tempWord, maxWord, maxCt = 1;
    var arr = str.toLowerCase().replace(/[^a-zA-Z ]/g,"").split(" ");

    for(var i = 0; i < arr.length; i++){
        tempWord = arr[i];
        ctObj = {}

        for(var j = 0; j <tempWord.length; j++){
          ctObj[tempWord[j]] = ctObj[tempWord[j]] || 0;
          ctObj[tempWord[j]]++;
        }
        for (var key in ctObj) {
          if (ctObj.hasOwnProperty(key)) {
              if (ctObj[key] > maxCt) {
                  maxCt = ctObj[key];
                  maxWord = tempWord;
              }
          }
        }
    }
      
    if (maxCt === 1) {
        return -1;
    } else {
        return maxWord;
    }
}
