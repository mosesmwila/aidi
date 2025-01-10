# AFLANG
- 😄 Find meaning ,understand local words & learn. 
- ⚡ We’re building language learning tools and spreading the Zambian Culture through technology

 - 🔭 Built with :

    + Web App : (Vue.js & Tailwind.css)
    + Backend : (PHP, Laravel & MySQL)
    + Mobile Apps : Flutter
----------------------------------------------------------------
## FEATURES
- Well Structured
- API (Tokens) Authorization
- Email Verification/Forgot Password
- Word Contribution (Adding/Suggesting/Updating)
- Random words/Trending Searches 
- Donation
- History
- Share
----------------------------------------------------------------
### Future (Considerations)

- [ ] Word Examples
- [ ] Word Pronunciations
- [ ] Categories (Based on Language)
- [ ] Proverbs
- [ ] Search
- [ ] Settings
- [ ] Word Contribution (Adding/Suggesting/Updating)

## ZLIP Dictionary Rest API
This is a dictionary rest API project including features like words,author,(category, search) , authentication using Sanctum (Token) from PHP Laravel framework.

## How to use ?
Follow these steps to get this project live

```
git clone https://github.com/mosesmwila/aflang.git
cd zlip
composer install

```
## Configure your .env file

```
DB_CONNECTION=mysql
DB_HOST=127.0.0.1
DB_PORT=3306
DB_DATABASE=db_name
DB_USERNAME=db_username
DB_PASSWORD=db_password

```

## Final steps

```
php artisan migrate
php artisan key:generate
http://localhost:8000

```
## Features
    1. Category (Add/Update/Remove/Search)
    2. Word (Add/Update/Remove/Search)
    3. Author (Register/Login/Logout)
    4. Comment (Add/Update/Remove)

## Authorization
    1. Category -> Needs to be authenticated for add/update/remove
    2. Word -> Needs to be authenticated for add/update/remove
    3. Author -> Needs to be authenticated for details/logout
    
## Endpoints
        
    1. Words
        1 ) Add -> /api/words/store 
        2 ) Update -> /api/v1/words/{id}/update 
        3 ) Remove -> /api/v1/words/{id}/remove 
        4 ) Show -> /api/v1/words/{id}/show 
        5 ) All -> /api/v1/words
        6 ) Search -> /api/v1/words/{keyword}/search
        
    2. Editor
        1 ) Register -> /api/register 
        2 ) Login -> /api/login
        3 ) Logout -> /api/logout
        

You can use Faker for generating random dummy data using the factories defined in this project.Just follow these steps
```
php artisan tinker
factory(App\ModelName::class,number_of_column)->create()
```

To test this API project you can use [Postman](https://www.postman.com/) application.For authorization purpose you need to add below headers
```
‘headers’ => [
    ‘Accept’ => ‘application/json’,
    ‘Authorization’ => ‘Bearer ‘.$accessToken,
]
```
## Thanks