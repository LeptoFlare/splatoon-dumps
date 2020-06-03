> This gist contains json documents with Splatoon 2 object data sourced from [loadout.ink](https://github.com/selicia/selicia.github.io/tree/master/en_US/data) for easy parsing.
> Each json document represents all objects of a particular object type.

### Changes from original source
- `weapons.json`:
  - The keys inside of `"stats"` have been converted to camelCase.
  - The weapon class key `"type"` has been renamed `"name"`
  - The weapon `"class"` key's value is now the id of the class.
  - Each of the the values in `minDamage`, `maxDamage`, and `mpuMaxDamage` that aren't maps have been casted into maps, under the key "damage".