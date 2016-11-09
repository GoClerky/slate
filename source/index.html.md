---
title: Clerky API Reference

language_tabs:
  - html
  - css
  - javascript

toc_footers:
  - <a href='#'>Sign Up for Clerky</a>
  - <a href='#'>Sign Up for a Developer Key</a>
  - <a href='https://github.com/tripit/slate'>Documentation Powered by Slate</a>

includes:
  - errors

search: true
---

<!---
  - shell
  - ruby
  - python
-->

# Introduction

Welcome to the Clerky API! You can use our API to access Kittn API endpoints, which can get information on various cats, kittens, and breeds in our database.

We have language bindings in Shell, Ruby, and Python! You can view code examples in the dark area to the right, and you can switch the programming language of the examples with the tabs in the top right.

This example API documentation page was created with [Slate](https://github.com/tripit/slate). Feel free to edit it and use it as a base for your own API's documentation.














# Website - Liquid Markup

## Objects


Welcome to the Clerky API! You can use our API to access Kittn API endpoints, which can get information on various cats, kittens, and breeds in our database.

We have language bindings in Shell, Ruby, and Python! You can view code examples in the dark area to the right, and you can switch the programming language of the examples with the tabs in the top right.



### Shop Object


```html
	Shop Example
```

> To authorize, use this code:

```html
{% if user %}
  Hello {{ user.name }}!
{% endif %}
```

The Kittn API uses the following error codes:


Shop Object | Meaning
---------- | -------
{{shop.name}} | Forbidden -- The kitten requested is hidden for administrators only
{{shop.support_email}} | Bad Request -- Your request sucks
{{shop.subdomain}} | Unauthorized -- Your API key is wrong






 
### Category Object



> To authorize, use this code:

```html
{% if user %}
  Hello {{ user.name }}!
{% endif %}
```


The Kittn API uses the following error codes:


Category Object | Description
---------- | -------
{{category.name}} | Bad Request -- Your request sucks
{{category.title}} | Bad Request -- Your request sucks
{{category.description}} | Unauthorized -- Your API key is wrong
{{category.parent}} | Unauthorized -- Your API key is wrong
{{category.slug}} | Unauthorized -- Your API key is wrong
{{category.image_url}} | Unauthorized -- Your API key is wrong
{{category.position}} | Unauthorized -- Your API key is wrong




### Product Object

> To authorize, use this code:

```html
{% if user %}
  Hello {{ user.name }}!
{% endif %}
```




The Kittn API uses the following error codes:

Product Object | Description
---------- | -------
{{product.id}} | Bad Request -- Your request sucks
{{product.title}} | Bad Request -- Your request sucks
{{product.image_url}} | Unauthorized -- Your API key is wrong
{{product.main_image}} | Unauthorized -- Your API key is wrong
{{product.overview}} | Unauthorized -- Your API key is wrong
{{product.description}} | Unauthorized -- Your API key is wrong
{{product.brand}} | Unauthorized -- Your API key is wrong
{{product.discount}} | Unauthorized -- Your API key is wrong
{{product.tags}} | Forbidden -- The kitten requested is hidden for administrators only
{{product.meta_description}} | Unauthorized -- Your API key is wrong
{{product.meta_keywords}} | Unauthorized -- Your API key is wrong
{{product.slug}} | Unauthorized -- Your API key is wrong
{{product.featured}} | Unauthorized -- Your API key is wrong
{{product.bestseller}} | Unauthorized -- Your API key is wrong
{{product.variants}} | Unauthorized -- Your API key is wrong
{{product.categories}} | Unauthorized -- Your API key is wrong
{{product.images}} | Unauthorized -- Your API key is wrong



### Variant Object


The Kittn API uses the following error codes:

Variant Object | Description
---------- | -------
{{variant.id}} | Forbidden -- The kitten requested is hidden for administrators only
{{variant.image_url}} | Bad Request -- Your request sucks
{{variant.title}} | Unauthorized -- Your API key is wrong
{{variant.description}} | Unauthorized -- Your API key is wrong
{{variant.price}} | Unauthorized -- Your API key is wrong
{{variant.recommended_price}} | Unauthorized -- Your API key is wrong
{{variant.sku}} | Unauthorized -- Your API key is wrong
{{variant.inventory_quantity}} | Unauthorized -- Your API key is wrong

  
  

### Page Object


The Kittn API uses the following error codes:


Page Object | Description
---------- | -------
{{page.id}} | Forbidden -- The kitten requested is hidden for administrators only
{{page.title}} | Bad Request -- Your request sucks
{{page.slug}} | Unauthorized -- Your API key is wrong
{{page.body}} | Not Found -- The specified kitten could not be found
{{page.image_url}} | Not Acceptable -- You requested a format that isn't json
{{page.tags}} | Not Acceptable -- You requested a format that isn't json
{{page.position}} | Method Not Allowed -- You tried to access a kitten with an invalid method
{{page.meta_title}} | Not Acceptable -- You requested a format that isn't json
{{page.meta_description}} | Not Acceptable -- You requested a format that isn't json
{{page.meta_keywords}} | Not Acceptable -- You requested a format that isn't json
{{page.layout}} | Not Acceptable -- You requested a format that isn't json




### Article Object


The Kittn API uses the following error codes:


Article Object | Description
---------- | -------
{{article.id}} | Forbidden -- The kitten requested is hidden for administrators only
{{article.title}} | Bad Request -- Your request sucks
{{article.slug}} | Unauthorized -- Your API key is wrong
{{article.content}} | Not Found -- The specified kitten could not be found
{{article.image_url}} | Not Acceptable -- You requested a format that isn't json
{{article.tags}} | Not Acceptable -- You requested a format that isn't json
{{article.seo_title}} | Method Not Allowed -- You tried to access a kitten with an invalid method
{{article.seo_description}} | Not Acceptable -- You requested a format that isn't json
{{article.published_at}} | Not Acceptable -- You requested a format that isn't json
  
  
  

The Kittn API uses the following error codes:



### Link Object


> To authorize, use this code:

```ruby
require 'kittn'

api = Kittn::APIClient.authorize!('meowmeowmeow')
```

```python
import kittn

api = kittn.authorize('meowmeowmeow')
```

```shell
```


Link Object | Description
---------- | -------
{{link.menu}} | Forbidden -- The kitten requested is hidden for administrators only
{{link.text}} | Bad Request -- Your request sucks
{{link.url}} | Unauthorized -- Your API key is wrong
{{link.position}} | Unauthorized -- Your API key is wrong
{{link.new_window}} | Unauthorized -- Your API key is wrong






### Review Object


> To authorize, use this code:

```ruby
require 'kittn'

api = Kittn::APIClient.authorize!('meowmeowmeow')
```

```python
import kittn

api = kittn.authorize('meowmeowmeow')
```

```shell
```


Review Object | Description
---------- | -------
{{review.rating}} | Forbidden -- The kitten requested is hidden for administrators only
{{review.review}} | Bad Request -- Your request sucks
{{review.reviewer}} | Unauthorized -- Your API key is wrong
{{review.image_url}} | Unauthorized -- Your API key is wrong




## Tags

Tags create the logic and control flow for templates. They are denoted by curly braces and percent signs: {% and %}.

The markup used in tags does not produce any visible text. This means that you can assign variables and create conditions and loops without showing any of the Liquid logic on the page.


{% if user %}
  Hello {{ user.name }}!
{% endif %}


> To authorize, use this code:

```html
{% if user %}
  Hello {{ user.name }}!
{% endif %}
```




## Filters





> To authorize, use this code:

```ruby
require 'kittn'

api = Kittn::APIClient.authorize!('meowmeowmeow')
```

```python
import kittn

api = kittn.authorize('meowmeowmeow')
```

```shell
```












# Email Templates

> To authorize, use this code:

```ruby
require 'kittn'

api = Kittn::APIClient.authorize!('meowmeowmeow')
```

```python
import kittn

api = kittn.authorize('meowmeowmeow')
```

```shell
# With shell, you can just pass the correct header with each request
curl "api_endpoint_here"
  -H "Authorization: meowmeowmeow"
```

```javascript
const kittn = require('kittn');

let api = kittn.authorize('meowmeowmeow');
```

> Make sure to replace `meowmeowmeow` with your API key.

Kittn uses API keys to allow access to the API. You can register a new Kittn API key at our [developer portal](http://example.com/developers).

Kittn expects for the API key to be included in all API requests to the server in a header that looks like the following:

`Authorization: meowmeowmeow`

<aside class="notice">
You must replace <code>meowmeowmeow</code> with your personal API key.
</aside>









# Merge Tags

## Get All Kittens

```ruby
require 'kittn'

api = Kittn::APIClient.authorize!('meowmeowmeow')
api.kittens.get
```

```python
import kittn

api = kittn.authorize('meowmeowmeow')
api.kittens.get()
```

```shell
curl "http://example.com/api/kittens"
  -H "Authorization: meowmeowmeow"
```

```javascript
const kittn = require('kittn');

let api = kittn.authorize('meowmeowmeow');
let kittens = api.kittens.get();
```

> The above command returns JSON structured like this:

```json
[
  {
    "id": 1,
    "name": "Fluffums",
    "breed": "calico",
    "fluffiness": 6,
    "cuteness": 7
  },
  {
    "id": 2,
    "name": "Max",
    "breed": "unknown",
    "fluffiness": 5,
    "cuteness": 10
  }
]
```

This endpoint retrieves all kittens.

### HTTP Request

`GET http://example.com/api/kittens`

### Query Parameters

Parameter | Default | Description
--------- | ------- | -----------
include_cats | false | If set to true, the result will also include cats.
available | true | If set to false, the result will include kittens that have already been adopted.

<aside class="success">
Remember — a happy kitten is an authenticated kitten!
</aside>

## Get a Specific Kitten

```ruby
require 'kittn'

api = Kittn::APIClient.authorize!('meowmeowmeow')
api.kittens.get(2)
```

```python
import kittn

api = kittn.authorize('meowmeowmeow')
api.kittens.get(2)
```

```shell
curl "http://example.com/api/kittens/2"
  -H "Authorization: meowmeowmeow"
```

```javascript
const kittn = require('kittn');

let api = kittn.authorize('meowmeowmeow');
let max = api.kittens.get(2);
```

> The above command returns JSON structured like this:

```json
{
  "id": 2,
  "name": "Max",
  "breed": "unknown",
  "fluffiness": 5,
  "cuteness": 10
}
```

This endpoint retrieves a specific kitten.

<aside class="warning">Inside HTML code blocks like this one, you can't use Markdown, so use <code>&lt;code&gt;</code> blocks to denote code.</aside>

### HTTP Request

`GET http://example.com/kittens/<ID>`

### URL Parameters

Parameter | Description
--------- | -----------
ID | The ID of the kitten to retrieve

