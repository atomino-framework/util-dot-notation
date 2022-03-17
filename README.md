# DotNotation utility

```php
DotNotation::extract(array $flattenedData):array;
DotNotation::flatten(array $hierarchicalData):array;
```

DotNotation converts hierarchical arrays between hierarchical format and dot-separated format.

Flattened dot-separated format:

```php
$data = [
  "alfa.beta.gamma" => "1",
  "alfa.beta.delta" => "2",
  "alfa.omega" => "3"
];
```

Hierarchical data extracted from the dot-separated format:

```php
$data = [
  "alfa" => [
    "beta" => [
      "gamma" => 1,
      "delta" => 2
    ],
    "omega" => 3
  ]
];
```
