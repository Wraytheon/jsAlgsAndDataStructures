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