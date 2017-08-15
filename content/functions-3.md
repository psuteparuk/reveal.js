### 3. Functions (cont.)

```ruby
class Quotation
  def remove_duplicated_referral
    user = self.try(:user)
    return if user.nil?
    self.referral_code = '' if user.has_referral?
      || user.motor_policy_bundles.one? { |policy| policy.is_from_referral? }
  end
end
```

```ruby
class Quotation
  def remove_duplicated_referral
    self.referral_code = '' if self.try(:user).try(has_referral?)
  end
end
```
<!-- .element: class="fragment" -->
