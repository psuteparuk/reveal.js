### 2. Naming (cont.)

Reveal Information / Avoid Disinformation <!-- .element: class="fragment" -->

```java
int ageList[] = new int[10]; // this is not a List
int ages[] = new int[10];

List<Integer> ageList = new ArrayList<>(); // avoid encoding types
List<Integer> ageGroup = new ArrayList<>();
```
<!-- .element: class="fragment" -->

<span class="fragment">Objects/Classes are <span class="text-primary">nouns</span>. Methods are <span class="text-primary">verbs</span>. Predicates should be prefixed with `is` or `has`.</span>

```typescript
const streetAddress: string = '1 Wall Rose, Paradis Island';
const customer: any = { name: 'Eren Jaeger', age: 15, type: 'human' };

const employeeName: string = employee.getName();
if (student.isMale() && student.hasCar())...
```
<!-- .element: class="fragment" -->
