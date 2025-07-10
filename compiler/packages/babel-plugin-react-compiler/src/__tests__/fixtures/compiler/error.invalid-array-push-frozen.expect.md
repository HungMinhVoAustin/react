
## Input

```javascript
function Component(props) {
  const x = [];
  <div>{x}</div>;
  x.push(props.value);
  return x;
}

```


## Error

```
Found 1 error:
Error: Updating a value used previously in JSX is not allowed. Consider moving the mutation before the JSX

error.invalid-array-push-frozen.ts:4:2
  2 |   const x = [];
  3 |   <div>{x}</div>;
> 4 |   x.push(props.value);
    |   ^ Updating a value used previously in JSX is not allowed. Consider moving the mutation before the JSX
  5 |   return x;
  6 | }
  7 |


```
          
      