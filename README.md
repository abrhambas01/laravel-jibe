# laravel-jibe
 > Test your api's directly in laravel without going to the browser or postman or fiddler or other tools for testing your api's


### Returns api responses without using the browser or using any api testing tools such as your browser, Postman and etc.. 



1. In the method in your controller make sure you're passing an argument to your ApiJibe instantiation.. the variable will be automatically translated to kebab case of what's the variable so $queryKey will be converted to query_key in your console

```
public function testMethod (){

$userId = auth()->user()->id ; 
$queryKey = ; 

new ApiJibe($userId ,  $queryKey ) ; 

....
the method you want to be returned such as..



}
```

2. Open your terminal / console,  make sure you named your routes.. refer to named routes..
```
  php artisan api:jibe name:route_name_here 
     or 
   php artisan api:jibe name:api.user.articles
``` 


it will ask you of the following inputs in your console depending in your controller's logic.. 

1. user_id : 3 
2. query_key : "gibber222"


