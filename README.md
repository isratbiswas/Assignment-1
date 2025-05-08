1. What are some differences between interfaces and types in TypeScript?
   Ans: Interfaces and types are similar, but they primarily apply to object types.
   We use interfaces to declare and define the shape of objects. Interfaces are powerful tools for describing the structure of object types.
   Example:
   interface Person {
   name: string;
   age: number;
   profession: string;
   gender: string;
   }

Types, on the other hand, can be used for both primitive types such as string, number, and boolean, as well as more complex types like objects and arrays.
Types are useful for improving code readability and can be easily used for type declarations.
Example:
type UserName = string
type IsAdmin =boolean
const userName : UserName = "Israt"
const isAdmin : IsAdmin = true

2.What is the use of the keyof keyword in TypeScript? Provide an example.

Ans: keyof is a keyword in TypeScript used to extract the key types from an object type.
When used with an explicit object type, keyof creates a union type of all the keys in that object.
Example:
type Student ={
id:number,
name: string,
email: string,
address: string,
ContactNo: number
}
type Student1= keyof Student
const person : Student1 = "email
