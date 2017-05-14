[![Published on webcomponents.org](https://img.shields.io/badge/webcomponents.org-published-blue.svg?style=flat-square)](https://beta.webcomponents.org/element/danielx/resettable-properties-behavior)

# ResettablePropertiesBehavior

`ResettablePropertiesBehavior` lets you easily reset polymer element properties to their default values.

`ResettablePropertiesBehavior` require properties that use this behavior to have a function as their value.

Set `resettable` to true for properties to reset them with `resetProperties`.
```javascript
data: {
  type: Array,
  resettable: true,
  value: function() {
    return [];
  }
}
```

Optionally set `resetGroups` to only reset a subset of resettable properties with `resetPropertyGroup(group)`.
```javascript
data: {
  type: Array,
  resettable: true,
  resetGroups: ['group-name'],
  value: function() {
    return [];
  }
}
```
