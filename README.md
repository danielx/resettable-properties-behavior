# ResettablePropertiesBehavior

`ResettablePropertiesBehavior` lets you easily reset polymer element properties to their default values.

To reset `Object` and `Array` types `ResettablePropertiesBehavior` require properties that use this behavior to have a function as their value.

Set `resettable` to true for properties to reset them with `resetProperties`.

    data: {
      type: Array,
      resettable: true,
      value: function() {
        return [];
      }
    }

Optionally set `resetGroups` to only reset a subset of resettable properties with `resetPropertyGroup(group)`.

    data: {
      type: Array,
      resettable: true,
      resetGroups: ['group-name'],
      value: function() {
        return [];
      }
    }
