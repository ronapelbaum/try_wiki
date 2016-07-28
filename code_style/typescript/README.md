#angular 1.x service in TypeScript
This is how to write your code

```typescript
module mymodule{
  /**
  * this is the the service class
  */
  export class MyService{
    //DI declaration - static on class
    static $inject = ['OtherService'];
    
    //this is the constructor for an instance of the service class
    constructor(private OtherService:OtherService){
    }
    
    public foo(){
    }
  }
  //register the service to angular
  angular.module('moduleName').service('MyService', MyService);
}
```
