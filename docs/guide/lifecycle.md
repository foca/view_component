---
layout: default
title: Lifecycle
parent: Guide
---

# Lifecycle

## `#before_render`

Define a `before_render` method to be called before a component is rendered, when `helpers` is able to be used:

```ruby
# app/components/example_component.rb
class ExampleComponent < ViewComponent::Base
  def before_render
    @my_icon = helpers.star_icon
  end
end
```
