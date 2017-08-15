### 3. Functions (cont.)

```ruby
class Quotation
  def remove_duplicated_referral
    user_id = self.user_id || self.try(:user).try(:id)
    if user_id
      if User
        .joins(:up_referral)
        .where(id: user_id)
        .where.not(referral: { id: nil })
        .exists? || MotorPolicyBundle
        .where(user_id: user_id)
        .where.not(referrer_id: nil)
        .exists?
        self.referral_code = ''
      end
    end
  end
end
```
