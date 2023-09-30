# Introduction

{% code title="find_missing.rb" lineNumbers="true" fullWidth="true" %}
```ruby
def find_missing(sequence)
  consecutive     = sequence.each_cons(2)
  differences     = consecutive.map { |a,b| b - a }
  sequence        = differences.max_by { |n| differences.count(n) }

  missing_between = consecutive.find { |a,b| (b - a) != sequence }

  missing_between.first + sequence
end

find_missing([2,4,6,10])
# 8
```
{% endcode %}

***

{% hint style="info" %}
asdfasdf

asdfasdf

asdfasdf
{% endhint %}

{% swagger method="get" path="" baseUrl="" summary="" %}
{% swagger-description %}

{% endswagger-description %}
{% endswagger %}
