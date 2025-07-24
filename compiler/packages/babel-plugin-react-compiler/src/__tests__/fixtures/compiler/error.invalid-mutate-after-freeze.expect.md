
## Input

```javascript
function Component(props) {
  let x = [];

  let _ = <Component x={x} />;

  // x is Frozen at this point
  x.push(props.p2);

  return <div>{_}</div>;
}

```


## Error

```
Found 1 error:
Error: Updating a value used previously in JSX is not allowed. Consider moving the mutation before the JSX

error.invalid-mutate-after-freeze.ts:7:2
   5 |
   6 |   // x is Frozen at this point
>  7 |   x.push(props.p2);
     |   ^ Updating a value used previously in JSX is not allowed. Consider moving the mutation before the JSX
   8 |
   9 |   return <div>{_}</div>;
  10 | }


```
          
      