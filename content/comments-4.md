### 4. Comments (cont.)

Focus on the <span class="text-primary">Why</span>, not the <span class="text-primary">What</span>

```typescript
const normalizePayloadKeys = (requestPayload: Object) => {
    return _.mapKeys(_.snakeCase, requestPayload);
};

const sendRequest = (request: Request) => {
    const payload: Object = request.payload;
    // conform to API payload key format
    const normalizedPayload = normalizePayloadKeys(payload);
    $.ajax({
        url: request.url,
        data: normalizedPayload,
    }).done(...);
    ...
};
```
