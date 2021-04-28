# Node Ecosystem, TDD, CI/CD

## Array.map() 
* creates a new array with the results of calling a function for every array element.

* calls the provided function once for each element in an array, in order.

* map() does not execute the function for array elements without values.

* this method does not change the original array.

* return array with the same length of the original array 

## Array.reduce()
* reduces the array to a single value.

* executes a provided function for each value of the array (from left-to-right).

* The return value of the function is stored in an accumulator (result/total).

* does not execute the function for array elements without values.

* This method does not change the original array.

## superagent()
``function getResultFromApi(req,res){``

  ``const url='http://hp-api.herokuapp.com/api/characters';``

  ``superagent.get(url).then(result=>{`` 

   ``return result.body.map(obj=>``

   ``new Hp(obj));``

  ``}).then(result=>{ res.render('index',{sendRes:result})``

  ``});``

``}``

## Promises Functions(Asynchronous)
* Executed first ==>show first Even if there is another promise not Executed yet , Depends on 
    1. which finsh his Executed first
    2. which have the request that  reaches first 
* you can worksomething else no need to wait the response , so try to do but not now
* your code continue work without stop 


### Are all callback functions considered to be Asynchronous? Why or Why Not?
- No, For instance, the callback used by Array#sort is not asynchronous, nor is the one used by String#replace.
The only way you know whether a callback is asynchronous is from its documentation. Typically, ones involving requests for external resources (ajax calls, for instance) are asynchronous, and others may or may not be.
- A callback can be used synchronously or asynchronously.