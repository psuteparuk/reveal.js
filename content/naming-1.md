### 2. Naming

Intention-Revealing <!-- .element: class="fragment" -->

```typescript
const d: Number; // elapsed time in days
const elapsedTimeInDays: Number;
```
<!-- .element: class="fragment" -->

```typescript
const getUsers = (list: [User]) => {
    const newList: [User] = [];
    list.forEach((x) => {
        if (x.age > 30) {
            newList.push(x);
        }
    });
    return newList;
};
```
<!-- .element: class="fragment" -->

```typescript
const AGE_THRESHOLD = 30;
const filterUsersByAge = (users: [User]) => {
    const filteredUsers: [User] = users
        .filter((user) => user.age > AGE_THRESHOLD);
    return filteredUsers;
};
```
<!-- .element: class="fragment" -->
