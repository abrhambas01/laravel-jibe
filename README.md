# laravel-jibe
 > Test your api's directly in laravel without going to the browser or postman or fiddler or other tools for testing your api's


### Returns api responses without using the browser or using any api testing tools such as your browser, Postman and etc.. 


1. Open your terminal / console
```
  php artisan api:jibe
``` 


2. In the method in your controller make sure you're passing an argument to your method


```
public function testMethod (){

$userId = auth()->user()->id ; 
$queryKey = ; 

new ApiJibe($userId ,  $queryKey ) ; 




}
```
