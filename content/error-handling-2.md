### 5. Error Handling (cont.)

```ruby
def get_commission(riskcost, car_code)
  if riskcost[:dry].try(:to_i).present? && riskcost[:dry].to_i != 0
    package_type = 'comprehensive'
  elsif riskcost[:fresh].try(:to_i).present? && riskcost[:fresh].to_i != 0
    package_type = 'dual_party'
  else
    package_type = 'third_party'
  end
  ...
end
```
