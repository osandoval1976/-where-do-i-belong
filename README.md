# -where-do-i-belong
Where-do-i-belong
//First with concat method num to arr
//second the sort() method to sort low and high
// the IndexOf to grab location of inserted num 

function getIndexToIns(arr, num) {
  // Find my place in this sorted array.
  let result = arr.concat(num)
  for(let i=0; i< result.length; i++){
    result[i]=result[i];
    result.sort(function(a,b){
       if(a > b){
         return 1;
       } 
       if(a < b) {
         return -1;
       }
       return 0;
        
  }); 
   
  }
  console.log(result);
  return result.indexOf(num)
}

getIndexToIns([40, 60], 50);
