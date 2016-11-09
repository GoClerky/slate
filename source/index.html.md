---
title: API Reference

language_tabs:
  - shell
  - html
  - css
  - ruby
  - python
  - javascript

toc_footers:
  - <a href='#'>Sign Up for Clerky</a>
  - <a href='#'>Sign Up for a Developer Key</a>
  - <a href='https://github.com/tripit/slate'>Documentation Powered by Slate</a>

includes:
  - errors

search: true
---

# Introduction

Welcome to the Clerky API! You can use our API to access Kittn API endpoints, which can get information on various cats, kittens, and breeds in our database.

We have language bindings in Shell, Ruby, and Python! You can view code examples in the dark area to the right, and you can switch the programming language of the examples with the tabs in the top right.

This example API documentation page was created with [Slate](https://github.com/tripit/slate). Feel free to edit it and use it as a base for your own API's documentation.














# Website - Liquid Markup

## Objects


Welcome to the Clerky API! You can use our API to access Kittn API endpoints, which can get information on various cats, kittens, and breeds in our database.

We have language bindings in Shell, Ruby, and Python! You can view code examples in the dark area to the right, and you can switch the programming language of the examples with the tabs in the top right.



  
The Kittn API uses the following error codes:


category Object | Explanation
---------- | -------
product.name | Bad Request -- Your request sucks
product.title | Bad Request -- Your request sucks
product.description | Unauthorized -- Your API key is wrong
product.parent | Unauthorized -- Your API key is wrong
product.slug | Unauthorized -- Your API key is wrong
product.image_url | Unauthorized -- Your API key is wrong
product.position | Unauthorized -- Your API key is wrong





The Kittn API uses the following error codes:


Product Object | Explanation
---------- | -------
product.id | Bad Request -- Your request sucks
product.title | Bad Request -- Your request sucks
product.image_url | Unauthorized -- Your API key is wrong
product.main_image | Unauthorized -- Your API key is wrong
product.overview | Unauthorized -- Your API key is wrong
product.description | Unauthorized -- Your API key is wrong
product.brand | Unauthorized -- Your API key is wrong
product.discount | Unauthorized -- Your API key is wrong
product.tags | Forbidden -- The kitten requested is hidden for administrators only
product.meta_description | Unauthorized -- Your API key is wrong
product.meta_keywords | Unauthorized -- Your API key is wrong
product.slug | Unauthorized -- Your API key is wrong
product.featured | Unauthorized -- Your API key is wrong
product.bestseller | Unauthorized -- Your API key is wrong
product.variants | Unauthorized -- Your API key is wrong
product.categories | Unauthorized -- Your API key is wrong
product.images | Unauthorized -- Your API key is wrong



The Kittn API uses the following error codes:


Variant Object | Meaning
---------- | -------
page.id | Forbidden -- The kitten requested is hidden for administrators only
page.image_url | Bad Request -- Your request sucks
page.title | Unauthorized -- Your API key is wrong
page.description | Unauthorized -- Your API key is wrong
page.price | Unauthorized -- Your API key is wrong
page.recommended_price | Unauthorized -- Your API key is wrong
page.sku | Unauthorized -- Your API key is wrong
page.inventory_quantity | Unauthorized -- Your API key is wrong

  
  



The Kittn API uses the following error codes:


Page Object | Meaning
---------- | -------
page.id | Forbidden -- The kitten requested is hidden for administrators only
page.title | Bad Request -- Your request sucks
page.slug | Unauthorized -- Your API key is wrong
page.body | Not Found -- The specified kitten could not be found
page.image_url | Not Acceptable -- You requested a format that isn't json
page.tags | Not Acceptable -- You requested a format that isn't json
page.position | Method Not Allowed -- You tried to access a kitten with an invalid method
page.meta_title | Not Acceptable -- You requested a format that isn't json
page.meta_description | Not Acceptable -- You requested a format that isn't json
page.meta_keywords | Not Acceptable -- You requested a format that isn't json
page.layout | Not Acceptable -- You requested a format that isn't json



The Kittn API uses the following error codes:


Article Object | Meaning
---------- | -------
page.id | Forbidden -- The kitten requested is hidden for administrators only
page.title | Bad Request -- Your request sucks
page.slug | Unauthorized -- Your API key is wrong
page.content | Not Found -- The specified kitten could not be found
page.image_url | Not Acceptable -- You requested a format that isn't json
page.tags | Not Acceptable -- You requested a format that isn't json
page.seo_title | Method Not Allowed -- You tried to access a kitten with an invalid method
page.seo_description | Not Acceptable -- You requested a format that isn't json
page.published_at | Not Acceptable -- You requested a format that isn't json
  
  
  

The Kittn API uses the following error codes:


Shop Object | Meaning
---------- | -------
page.name | Forbidden -- The kitten requested is hidden for administrators only
page.support_email | Bad Request -- Your request sucks
page.subdomain | Unauthorized -- Your API key is wrong



Link Object | Meaning
---------- | -------
page.menu | Forbidden -- The kitten requested is hidden for administrators only
page.text | Bad Request -- Your request sucks
page.url | Unauthorized -- Your API key is wrong
page.position | Unauthorized -- Your API key is wrong
page.new_window | Unauthorized -- Your API key is wrong





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

