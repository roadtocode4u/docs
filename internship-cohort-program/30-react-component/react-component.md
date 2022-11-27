# React Component 

### Components 

```
Component is reusable code blocks.
```

**Syntax**

```js
  function Home()
  {
        return(
            <div>
                <h1>Heading 1</h1>
                 <h2>Heading 2</h2>
            </div>
            );
  }
  export default Home;
```

**Empty Elements <> </>**

```js
  function Home()
  {
        return(
            <>
                <h1>Heading 1</h1>
                 <h2>Heading 2</h2>
            </>
            );
  }
  export default Home;
```

**💡Important Note**

```
If we want to apply the CSS classes, we use className attribute instead of class in React.
```

**Named Export components Syntax:**

```js
export function Name()
{
    return(<> </>)
}
```

**Named import components Syntax:**

```js
 import {Name} from fileName;
```

**default Export components Syntax:**

```js
    export default function Name()
    {
        return(<> </>)
    }
```

**default import components Syntax:**

```js
    import Name from file
```
