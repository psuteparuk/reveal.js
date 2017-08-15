### 5. Error Handling

- Clean code must be robust. <!-- .element: class="fragment" -->
- Always think of all the corner cases and handle all possible events within the function. <!-- .element: class="fragment" -->

```ruby
def get_commission(riskcost, car_code)
  if riskcost[:dry] != 0
    package_type = 'comprehensive'
  elsif riskcost[:fresh] != 0
    package_type = 'dual_party'
  else
    package_type = 'third_party'
  end
  ...
end
```
<!-- .element: class="fragment" -->
