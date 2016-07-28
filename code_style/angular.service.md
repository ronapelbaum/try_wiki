#angular 1.x service

this is how to write your service:

```javascript
(function(){
  /**
  * this is the constructor for an instance of the service class
  */
  function MyService(OtherService){
    this.foo = function(){
    };
  }
  //DI declaration - static on class
  MyService.$inject = ['OtherService'];
  
  //register the service to angular
  angular.module('moduleName').service('MyService', MyService);
})();
```
