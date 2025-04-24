
Table product_image {
  image_id  integer [primary key]
  product_id  varchar(50)
  image_url  varchar(50)
}

Table color {
  color_id integer [primary key]
  color_name varchar(50)
}

Table product_category {
  category_id   integer [primary key]
  category_name  varchar(50)
}

Table product {
  product_id   integer [primary key]
  name  varchar(50)
  brand_id  integer
  base_price integer
}

Table product_item {
  item_id integer [primary key]
  product_id  integer
  variation_id integer
  quantity integer
}

Table brand{
  brand_id integer [Primary Key]
  brand_name vacher

}

Table product_variation {
    variation_id integer [Primary Key]
    product_id integer 
    size_id integer 
    color_id integer 

}

Table size_category {
  size_category_id integer [Primary Key]
  category_name vacher(50)

}

Table size_option {
    size_id  integer [Primary Key]
    size_category_id integer 
    size_value integer

}

Table product_attribute {
    Attribute_id integer [Primary Key]
    product_id integer 
    attribute_type_id integer 
    attribute_value integer

}

Table attribute_category{
  attribute_category_id integer [Primary Key]
  category_name vacher(50)

}

Table attribute_type {
    attribute_type_id integer [Primary Key]
    attribute_category_id integer
    type_name vacher(50)

}


