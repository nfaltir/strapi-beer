## Backend

- start server `npm run develop`

## Strapi Config

- in public tab, navigate to roles, check `find, findone` (for now) to enable GET routes
- navigate towards `Users` and create a use, confirmed = true, role = authenticated this allows POST/PUT and DELETE routes

<br>

### Post

<br>

user: TestUser
pass: "$dBkhzHXp2ceQ#$"
<br>

```json

route: http://localhost:1337/api/auth/local

postman>body>raw>json

{
  "identifier": "TestUser",
  "password": "$dBkhzHXp2ceQ#$"
}
```

<br>

## graphql

<br>

- install graphql in strapi panel marketplace, copy link run it in terminal
- install apollo `npm install @apollo/client graphql`

```graphql

allReviews

query GetReviews {
  reviews {
    data {
      id
      attributes {
        title
        rating
        body
      }
    }
  }
}

```

<br>

```graphql
singleReviews

query GetReview($id: ID!) {
    review(id: $id) {
      data {
        id
        attributes {
          title
          rating
          body
        }
      }
    }
  }

```

<br>

## Adding A New Content type

<br>

- from content builder create a new collection type
- name it category
- create 1 field, name it 'name' and in advanced settings label it required
- create test fields ['IPA', 'Stout', 'Lager']
- Associate it `Reviews` collection. make it realational
- click on `Reviews` collection, select another field type, choose `relation` option
- select `Reviews has and belongs to many categories` model relationship
