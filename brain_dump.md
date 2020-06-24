# components

## Items
### Configs
```
Items::restaurant_menu
----------
structure_graph: graph::simple_restaurant_types
item_fields: { tag::type::location => fields::location }
```
### Contents

## Tags
### Configs
```
tag::type::location
tag::type::category
tag::type::product
```
## Graph
### Configs
```
graph::simple_restaurant_types
----------
tag::type::location -> {tag::type::category, tag::type::product}
tag::type::category -> {tag::type::category, tag::type::product}
tag::type::product -> {}
```

## Fields
### configs
```
fields::location
----------
name: text
photo: image
address: location
features: tags::location_features
```
