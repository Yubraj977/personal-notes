## Data Types
![Screenshot (8)](https://github.com/Yubraj977/personal-notes/assets/112848654/dc6cac9a-426e-42dd-9feb-80a4a33ccaea)
```ts
// number
// boolean
// any = when no any type is passed like let a;  this  can have anything
```

## Function
##### Function argumests should have the typechecking
```typescript
function add(name: string, email: string, isPaid: boolean=false){
we are making the ispaid deafult false so it doesnt make problem later in the file
}

function return(num:number):number{
return "hello"
// This saids return only number string is now allowded
}
function handeleError(errmsg: string):void{
return "hello"
//this is the err cause void means return nothing
// never in place of the void return but doesnt matter
}

```

## Objects
```typescript
// Function returning Objects
function create():{name:string, price:number}{

}
```
## Type Alaises
```typescript
type User={
name:string,
email:string,
isActive:boolean
}
type Mysting:string // Making the own data type

function createuser(user:User):User{
return {name:"hero",email:"email@gamil",isActive:true}
}
createuser({name:"khatri",email:"this@gmail.com",isActive:true})

type new={
readonly _id:string //nobody can change this
name:string
}
let person:new={
_id:"dfasdfa",
name:"This is the name"
gender?:boolean // question mark here mean that we can put or leave empty too
}
person.name="this is new name"
person._id="dfadf" // this is not avilavle
```

```typescript
type CardNumber={
cardNumber:string
}

type cardData={
cardData:string
}


// It is combining and when we are dong cardDetials we should have the cardnumber and cardData
type cardDetails=cardNumber&cardDate&{
dvv:string
}
```

## Arrays
```typescript
const superHeros:string[]=[] // This is telling we have the array of strings
const superHeros:number[][]=[] // Array under array should be the number
const superHeros:costumDatatypes[]=[] // This is telling we have costum type
const superHeros:Array<number>=[] // This is telling we have the array of number
```

## Union in Typescript  May be this value or this like num or string
```typescript
let value:number|string=33  //number or string
let data:(number| string)[]=[1,2,"hello"]
let seathave:"window"|"Front"|"back" // only can have jsut these theree values
```
