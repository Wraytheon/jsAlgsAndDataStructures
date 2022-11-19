# All Notes

## 20 - Create a Module Script
- `script type="module"` is necessary for exporting/importing parts of code from separate files


## 21 - Use export to Share a Code Block
- Can export in two formats:
```javascript
export const result = (x) => {return x}
```
 ```javascript
const result = (x) => {
  return x
}
export { result }

```

## 22 - Reuse JavaScript Code Using import
```javascript
import { add } from './math_functions.js';
```
- The relative file path (./ tells the import that the js file is in the same folder as the current file) and file extension are required to import this way
- Can import several at a time using commas 
```javascript
import { add, subtract }
```

## 23 - Use * to Import Everything from a File
- The '*' allows you to import everything from a file
  - creates an object with whatever variable name you choose and this object contains all of the exports
  - Can access functions like any object property
  ```javascript
  myMathModule.add(2,3);
  ```

## 24 - Create An Export Fallback With Export Default
- Named exports vs default exports
  - Named exports:
    - Allows you to export several functions/variables
    - ```javascript
      export default function add(x,y) {
        return x + y;
      }
  - Default exports: usually used this syntax if only one value is being exported from a file. It is also used to create a fallback value for a file or module.
    - Cannot be used with let, var, or const
    - Can only have one value be a default export 
    - Default: anonymous function
      - ```javascript
        export default function(x, y) {
        return x + y;
        }
        ```
