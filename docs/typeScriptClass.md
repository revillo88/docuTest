## Beispiel classe

``` ts
 import './style.css';
export class Peter <T, E>implements Gender <T, E > {
  namen:T;
  nachnamen:string;
  alter:E;

  constructor(){
  }
  getAlter():E{
    return this.alter
  }
  setAlter(alter:E):void{
    this.alter = alter;
  }
  setName(namen:T):void{
      this.namen = namen
  }
  getNamen(): T{
    return this.namen
  }
}
```
## Beispiel Interface

```ts
export interface Gender<T, E>{

  setName(namen:T):void;
  getNamen(): T;
  getAlter(): E;
  setAlter(alter:E):void;

}

// Write TypeScript code!
const appDiv: HTMLElement = document.getElementById('app');

//let lele : Peter = new Peter('Peter', 'Maiyer', 42);
let lele : Gender<string, number >= new Peter();
lele.setAlter(400);
lele.setName('sdsd')

console.log(typeof lele)

console.log (lele.getNamen())
appDiv.innerHTML = `<h1>TypeScript Starter</h1>`;
 
```