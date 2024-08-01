# FSWDT26
day26
<!DOCTYPE html>
<html>
    <head>
    <title>Promises,Aync Await and DOM tree</title>
</head>
<body>
    <h2>Promises,Aync Await and DOM tree</h2>
    <script src="./day27.js"></script>
</body>
</html>
// var myPromise= new Promise((resolve,reject)=>{
//     setTimeout(function(){
//         resolve("sucess");
//     },3000);

// setTimeout (function(){
//     reject("error");
// },3000);
// });
// myPromise
// // .then((data)=>(data+="hey"))
// // first thhen will only be execued first
// .then((data)=>{console.log(data)})
// .then((data)=>{
//     data="hey"+data;
//     return data;
// })
// .catch((error)=>{console.log(error)});

// Asyn and Awat
// Asynchronous manner operation is usally followed by our compiler in such scenarious we use await for certain operations to carry out eg:Bank transfer
// setTimeout(function(){
//     console.log("1");
// },2000);
// console.log("2");

// Second method other then using then catch we used async await 
var myPromise=new Promise((resolve,reject)=>{
    resolve("sucess");
});
// var getourPromise= async()=>{
//     var getourPromiseresult =await myPromise;
//     console.log("getourPromiseresult",getourPromiseresult);
// }
// getourPromise();

// Third method here we used try and catch method
var getourPromise=async () => {
    try{
    getourPromiseResult=await myPromise;
    console.log(getourPromiseResult);
    }
    catch(error){
        console.log(error);
    }
};
getourPromise();
