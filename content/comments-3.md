### 4. Comments (cont.)

Focus on the <span class="text-primary">Why</span>, not the <span class="text-primary">What</span>

```typescript
// May object keys to snake case
const mapKeysToSnakeCase = (obj: Object) => {
    return _.mapKeys(_.snakeCase, obj);
};

const sendRequest = (request: Request) => {
    const payload: Object = request.payload;
    // Map the keys to snake case before sending the request
    const payloadWithSnakeCaseKeys = mapKeysToSnakeCase(payload);
    $.ajax({
        url: request.url,
        data: payloadWithSnakeCaseKeys,
    }).done(...);
    ...
};
```
<!-- .element: class="fragment" -->
