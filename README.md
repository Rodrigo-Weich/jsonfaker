<p align="center">
  <img src="https://raw.githubusercontent.com/Rodrigo-Weich/jsonfaker/main/content/logo.png">
</p>

<p align="center">
  <a href="https://nodejs.org/">
    <img src="https://img.shields.io/badge/NodeJS-1.15-blue.svg">
  </a>
  <a href="https://github.com/Rodrigo-Weich/jsonfaker">
    <img src="https://img.shields.io/badge/Release-1.X-red.svg">
  </a>
    <a href="https://opensource.org">
    <img src="https://img.shields.io/badge/Open%20Source-%E2%9D%A4-brightgreen.svg">
  </a>
</p>

<p align="center">
  JSONFaker is an app created in NodeJS to create custom api tests, following a simple guidance in JSON format, the app returns fictitious data to the user according to their needs.
</p>

## How to Install
```sh
# Get this repository
$ git clone git@github.com:Rodrigo-Weich/jsonfaker.git

# Go into the repository
$ cd jsonfaker/

# Run (NPM)
$ npm run dev
# Run (Yarn)
$ yarn dev
```

## Basic Usage

|Resquest type|Format|Limit|
|--------|-----|----|
|GET|Body JSON|Unlimited|

```json
{
  "your_custom_key": "desired_value_that_will_be_returned",
  "your_custom_key_level_two": {
    "your_custom_key": "other_desired_value_that_will_be_returned"
  }
}
```

### Examples

##### Simple Request

```json
{
  "first_name": "name_firstName"
}
```
##### Simple Response
```json
{
  "first_name": "Fannie"
}
```


##### Advanced Request

```json
{
  "first_name": "name_firstName",
  "last_name": "name_lastName",
  "age": "random_number",
  "phone": "phone_phoneNumber",
  "username": "internet_userName",
  "emails": {
  "one": "internet_email",
  "two": "internet_exampleEmail"
  },
  "website": "internet_domainName",
  "description": "lorem_paragraph",
  "last_visit": {
  "ip": "internet_ip",
  "mac": "internet_mac",
  "userAgent": "internet_userAgent",
  "date": "date_past"
  },
  "images": {
  "image": "image_image",
  "avatar": "image_avatar",
  "url": "image_imageUrl",
    "abstract": "image_abstract",
    "animals": "image_animals",
    "business": "image_business",
    "cats": "image_cats",
    "city": "image_city",
    "food": "image_food",
    "nightlife": "image_nightlife",
    "fashion": "image_fashion",
    "people": "image_people",
    "nature": "image_nature",
    "sports": "image_sports",
    "technics": "image_technics",
    "transport": "image_transport"
  }
}
```
##### Advanced Response
```json
{
  "first_name": "Fannie",
  "last_name": "Stokes",
  "age": "89057",
  "phone": "(834) 297-0011 x02393",
  "username": "Esteban.Hermann",
  "emails": {
    "one": "Yolanda_Bahringer@yahoo.com",
    "two": "Verlie_Pollich@example.net"
  },
  "website": "liliana.name",
  "description": "Quam ipsa doloribus beatae corrupti sint. Eos aperiam id porro accusantium impedit magnam voluptatem. Molestiae veniam in aut a quo impedit qui ratione. Vel veritatis ut consequatur vitae voluptatem iusto et cum. In qui voluptates velit eos minus. Enim et vitae sed laudantium.",
  "last_visit": {
    "ip": "232.146.14.156",
    "mac": "fc:a9:39:ed:07:27",
    "userAgent": "Mozilla/5.0 (Macintosh; Intel Mac OS X 10_7_5 rv:6.0; BG) AppleWebKit/533.1.0 (KHTML, like Gecko) Version/6.0.3 Safari/533.1.0",
    "date": "2020-05-23T00:59:03.505Z"
  },
  "images": {
    "image": "http://placeimg.com/640/480/transport",
    "avatar": "https://s3.amazonaws.com/uifaces/faces/twitter/nathalie_fs/128.jpg",
    "url": "http://placeimg.com/640/480/transportUrl",
    "abstract": "http://placeimg.com/640/480/abstract",
    "animals": "http://placeimg.com/640/480/animals",
    "business": "http://placeimg.com/640/480/business",
    "cats": "http://placeimg.com/640/480/cats",
    "city": "http://placeimg.com/640/480/city",
    "food": "http://placeimg.com/640/480/food",
    "nightlife": "http://placeimg.com/640/480/nightlife",
    "fashion": "http://placeimg.com/640/480/fashion",
    "people": "http://placeimg.com/640/480/people",
    "nature": "http://placeimg.com/640/480/nature",
    "sports": "http://placeimg.com/640/480/sports",
    "technics": "http://placeimg.com/640/480/technics",
    "transport": "http://placeimg.com/640/480/transport"
  }
}
```

## Available methods
#### Address

- address_zipCode
- address_city
- address_cityPrefix
- address_citySuffix
- address_streetName
- address_streetAddress
- address_streetSuffix
- address_streetPrefix
- address_secondaryAddress
- address_county
- address_country
- address_countryCode
- address_state
- address_stateAbbr
- address_latitude
- address_longitude
- address_direction
- address_cardinalDirection
- address_ordinalDirection
- address_nearbyGPSCoordinate
- address_timeZone

#### Commerce

- commerce_color
- commerce_department
- commerce_productName
- commerce_price
- commerce_productAdjective
- commerce_productMaterial
- commerce_product
- commerce_productDescription
- company_suffixes
- company_companyName
- company_companySuffix
- company_catchPhrase
- company_bs
- company_catchPhraseAdjective
- company_catchPhraseDescriptor
- company_catchPhraseNoun
- company_bsAdjective
- company_bsBuzz
- company_bsNoun

#### Database

- database_column
- database_type
- database_collation
- database_engine

#### Date

- date_past
- date_future
- date_recent
- date_soon
- date_month
- date_weekday

#### Finance

- finance_account
- finance_accountName
- finance_routingNumber
- finance_mask
- finance_amount
- finance_transactionType
- finance_currencyCode
- finance_currencyName
- finance_currencySymbol
- finance_bitcoinAddress
- finance_litecoinAddress
- finance_creditCardNumber
- finance_creditCardCVV
- finance_ethereumAddress
- finance_iban
- finance_bic
- finance_transactionDescription

#### Git

- git_branch
- git_commitEntry
- git_commitMessage
- git_commitSha
- git_shortSha

#### Hacker

- hacker_abbreviation
- hacker_adjective
- hacker_noun
- hacker_verb
- hacker_ingverb
- hacker_phrase

#### Helpers

- helpers_randomize
- helpers_slugify
- helpers_replaceSymbolWithNumber
- helpers_replaceSymbols
- helpers_replaceCreditCardSymbols
- helpers_shuffle
- helpers_createCard
- helpers_contextualCard
- helpers_userCard
- helpers_createTransaction

#### Image

- image_image
- image_avatar
- image_imageUrl
- image_abstract
- image_animals
- image_business
- image_cats
- image_city
- image_food
- image_nightlife
- image_fashion
- image_people
- image_nature
- image_sports
- image_technics
- image_transport
- image_dataUri

#### Internet

- internet_avatar
- internet_email
- internet_exampleEmail
- internet_userName
- internet_protocol
- internet_url
- internet_domainName
- internet_domainSuffix
- internet_domainWord
- internet_ip
- internet_ipv6
- internet_userAgent
- internet_color
- internet_mac
- internet_password

#### Lorem

- lorem_word
- lorem_words
- lorem_sentence
- lorem_slug
- lorem_sentences
- lorem_paragraph
- lorem_paragraphs
- lorem_text
- lorem_lines

#### Name

- name_firstName
- name_lastName
- name_findName
- name_jobTitle
- name_prefix
- name_suffix
- name_title
- name_jobDescriptor
- name_jobArea
- name_jobType

#### Phone

- phone_phoneNumber
- phone_phoneNumberFormat
- phone_phoneFormats

#### Random

- random_number
- random_float
- random_arrayElement
- random_arrayElements
- random_objectElement
- random_uuid
- random_boolean
- random_word
- random_words
- random_image
- random_locale
- random_alpha
- random_alphaNumeric
- random_hexaDecimal

#### System

- system_fileName
- system_mimeType
- system_commonFileType
- system_commonFileExt
- system_fileType
- system_directoryPath
- system_filePath
- system_semver

#### Time

- time_recent

#### Vehicle

- vehicle_vehicle
- vehicle_manufacturer
- vehicle_model
- vehicle_type
- vehicle_fuel
- vehicle_vin
- vehicle_color