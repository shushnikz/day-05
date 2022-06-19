# day-05
Do the below programs in anonymous function & IIFE
Print odd numbers in an array   
                                                                                                                        
            function odd(arr){
 var arr1=[];
 for(var i=0;i<arr.length;i++){
  if(arr[i]%2!==0){
  arr1.push(arr[i]);
 }
 }
  return arr1;
 }
 console.log(odd([1,2,3,4,5]));                                                                                                                                                                 }


Convert all the strings to title caps in a string array

function titleCase(str) {
  return str.toLowerCase().split(' ').map(function(word) {
    return (word.charAt(0).toUpperCase() + word.slice(1));
  }).join(' ');
}
console.log(titleCase("converting string to titile case"));
 


Sum of all numbers in an array

function sumofarray(arr){
 var sum=0;
 for(var i=0;i<arr.length;i++){
 sum += arr[i];
 }
 return sum;
 }
 console.log(sumofarray([1,2,3,4,5]));
 

Return all the prime numbers in an array
function sumPrimes(num){
  var arr1=[];
  for (let i = 2; i <num.length; i++) {
    if(num[i]%2!=0){
    arr1.push(num[i]);
  }
  }
  return arr1;
  }
  console.log(sumPrimes([1,2,3,4,5,6,7,8]));


Return all the palindromes in an array

function palindrome(num){
  var temp=[];
  let str = num.slice(0)
  let pal = str.toString().split("").reverse().join("") 
   console.log(pal);

  for(var i=0;i<num.length;i++){
  for(var j=0;j<pal.length;j++){
  if (num[i] == pal[k]) {
   temp.push(num[i])
 }
 }
 }
 return temp;
 }
 console.log(palindrome([1,2,3,2,4]));


Return median of two sorted arrays of the same size
function getMedian(ar1, ar2, n)
{
    var i = 0;
    var j = 0;
    var count;
    var m1 = -1, m2 = -1;
    for (count = 0; count <= n; count++)
    {
        
        if (i == n)
        {
            m1 = m2;
            m2 = ar2[0];
            break;
        }
        else if (j == n)
        {
            m1 = m2;
            m2 = ar1[0];
            break;
        }
        
        if (ar1[i] <= ar2[j])
        {
            m1 = m2; 
            m2 = ar1[i];
            i++;
        }
        else
        {
            m1 = m2; 
            m2 = ar2[j];
            j++;
        }
         return (m1 + m2)/2;
}

}
console.log(getMedian([1,2,3,4,5],[3,4,6,7,8],5));


Remove duplicates from an array

function unique(a) {
   return Array.from(new Set(a));
}
console.log(unique([1,2,3,4,4,5,5,2,1]));


Rotate an array by k times

function arrayRotate(arr, reverse) {
  if (reverse) arr.unshift(arr.pop());
  else arr.push(arr.shift());
  return arr;
}
console.log(arrayRotate([1,2,3,4,5]));


Do the below programs in arrow functions
Print odd numbers in an array

var odd=(arr)=>{
 var arr1=[];
 for(var i=0;i<arr.length;i++){
  if(arr[i]%2!==0){
  arr1.push(arr[i]);
 }
 }
  return arr1;
 }
 console.log(odd([1,2,3,4,5]))

Convert all the strings to title caps in a string array
var titleCase=(str)=>{
  return str.toLowerCase().split(' ').map(function(word) {
    return (word.charAt(0).toUpperCase() + word.slice(1));
  }).join(' ');
}
console.log(titleCase("converting string to titile case"));



Sum of all numbers in an array

var sumofarray=(arr)=>{
 var sum=0;
 for(var i=0;i<arr.length;i++){
 sum += arr[i];
 }
 return sum;
 }
 console.log(sumofarray([1,2,3,4,5]));

Return all the prime numbers in an array

var sumPrimes=(num)=>{
  var arr1=[];
  for (let i = 2; i <num.length; i++) {
    if(num[i]%2!=0){
    arr1.push(num[i]);
  }
  }
  return arr1;
  }
  console.log(sumPrimes([1,2,3,4,5,6,7,8]));

Return all the palindromes in an array

var palindrome=(num)=>{
  var temp=[];
  let str = num.slice(0)
  let pal = str.toString().split("").reverse().join("") 
   console.log(pal);

  for(var i=0;i<num.length;i++){
  for(var j=0;j<pal.length;j++){
  if (num[i] == pal[k]) {
   temp.push(num[i])
 }
 }
 }
 return temp;
 }
 console.log(palindrome([1,2,3,2,4]));
  
