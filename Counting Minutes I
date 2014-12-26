/***************************************************************************************
*                                                                                      *
*                  CODERBYTE BEGINNER CHALLENGE                                        *
*                                                                                      *
*  Counting Minutes I                                                                  *
*  Using the JavaScript language, have the function CountingMinutesI(str) take the     *
*  str parameter being passed which will be two times (each properly formatted with    *
*  a colon and am or pm) separated by a hyphen and return the total number of minutes  *
*  between the two times. The time will be in a 12 hour clock format. For example:     *
*  if str is 9:00am-10:00am then the output should be 60. If str is 1:00pm-11:00am     *
*  the output should be 1320.                                                          *
*                                                                                      *
*  SOLUTION                                                                            *
*  Sometimes it pays to spend more time mapping out all the possibilites you might     *
*  face in solving a problem before you start programming. This challenge will have    *
*  4 possible scenarios. They are:                                                     *
*    a) both have same ampm values and first time is after second time                 *
*    b) both have same ampm values and the first time is before second time            *
*    c) have different ampm times and time1 is am                                      *
*    d) have different ampm times and time2 is pm                                      *
*                                                                                      *
*  I am going to use an object to represent both times simply because I like to use    *
*  words like hours, mins, and ampm instead of referring to an array index. To parse   *
*  the str into the two time objects I created a separate function. Now that I have    *
*  my 2 time object I just need to create a series of IF statements to correspond to   *
*  the 4 scenarios listed above to calculate the timeDiff.                             *
*                                                                                      *
*  Steps for solution                                                                  *
*    1) Use RegExp pattern to search string for pattern a...b                          *
*    2) If found return true                                                           *
*    3) Else return false                                                              *
*                                                                                      *
***************************************************************************************/
function CountingMinutesI(str) { 
    var time1Obj = {}, time2Obj = {}, timeDiff;
    
    time1Obj = setTimeObject(str, 0);
    time2Obj = setTimeObject(str, 1);
    
    if (time1Obj.ampm == time2Obj.ampm && time1Obj.tot > time2Obj.tot) {
        timeDiff = (((12 - time1Obj.hours + 12) * 60) - (time1Obj.mins)) + ((time2Obj.hours * 60) + time2Obj.mins);
    } 
    else if (time1Obj.ampm == time2Obj.ampm && time1Obj.tot < time2Obj.tot) {
        timeDiff = ((time2Obj.hours * 60) + time2Obj.mins) - ((time1Obj.hours * 60) + time1Obj.mins);
    }
    else if (time1Obj.ampm !== time2Obj.ampm && time1Obj.ampm === "am") {
        timeDiff = (((12 - time1Obj.hours) * 60) - time1Obj.mins) + ((time2Obj.hours * 60) + time2Obj.mins);
    }
    else { 
        timeDiff = (((12 - time1Obj.hours) * 60) - time1Obj.mins) + ((time2Obj.hours * 60) + time2Obj.mins);
    }

    return timeDiff;
}
    
function setTimeObject(str, num) {
    var arr = str.split("-");
    var tObject = {};
    
    tObject.hours = Number(arr[num].slice(0,arr[num].length-2).split(":")[0]);
    tObject.mins = Number(arr[num].slice(0,arr[num].length-2).split(":")[1]);
    tObject.ampm = arr[num].slice(-2);
    tObject.tot = tObject.hours * 100 + tObject.mins;
    
    return tObject;
}
