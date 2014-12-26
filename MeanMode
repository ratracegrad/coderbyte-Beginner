/***************************************************************************************
*                                                                                      *
*                  CODERBYTE BEGINNER CHALLENGE                                        *
*                                                                                      *
*  MeanMode                                                                            *
*  Have the function MeanMode(arr) take the array of numbers stored in arr and         *
*  return 1 if the mode equals the mean, 0 if they don't equal each other              *
*  (ie. [5, 3, 3, 3, 1] should return 1 because the mode (3) equals the mean (3)).     *
*  The array will not be empty, will only contain positive integers, and will not      *
* contain more than one mode.                                                          *
*                                                                                      *
*  SOLUTION                                                                            *
*  Since it is possible that I will want a function that will calculate the mean or    *
*  mode in the future, I decided to create separate functions for each. The mean is    *
*  calculated by the average of all values in the array. The mode is the number that   *
*  exists the most in the array. My solution is to call my two functions and then      *
*  compare to see if they are equal and if so return 1 else return 0.                  *
*                                                                                      *
*  Steps for solution                                                                  *
*    1) Create separate functions for getMean and getMode                              *
*    2) Compare the values returned from the two functions                             *
*    3) If values are equal return 1 else return 0                                     *
*                                                                                      *
***************************************************************************************/
function MeanMode(arr) { 

  var myMean, myMode;
  
  myMode = getMode(arr);
  myMean = getMean(arr);
  
  if(myMode == myMean) {
    return 1;
  } else {
    return 0;
  }
         
}

function getMean(arr) {
    var sum = 0, mean;
 
	for (var i = 0; i < arr.length; i++){
		sum = sum + arr[i];
	}
	mean = sum / arr.length;
    
    return mean;
}


function getMode(arr) {
    var ctObj = {}, mode, maxCt = 1;
    
    arr.sort(function(a, b) {return a - b;});
    
    for (var i = 0; i < arr.length; i++){
		ctObj[arr[i]] = ctObj[arr[i]] || 0;
        ctObj[arr[i]]++;
	}
    
    for (var key in ctObj) {
        if (ctObj.hasOwnProperty(key)) {
            if (ctObj[key] > maxCt) {
                maxCt = ctObj[key];
                mode = key;
            }
        }
    }
    
    return mode;
}
