# MongoDB Laravel 8 Example

## Installation

At the current moment there are no instructions for installing `mongodb` within this repo, you will have to install and configure it yourself.

Make sure to configure your `.env` to `DB_CONNECTION=mongodb` and `DB_PORT=27017` (If using the default mongodb ports)

Install and serve this laravel application as you wish.

## Usage

Functionality and routes can be found in `api.php` and `PostController::class` within the usual controllers folder. The model `Post::class` will show you an example of show I figured the Laravel Model class to use MongoDB collections.

### POST /api/posts/

```
curl --request POST \
  --url http://localhost/api/posts/ \
  --header 'Content-Type: application/json' \
  --data '{
  "title" : "First Post",
  "body" : "This is my first post.",
  "slug" : "first-blog-post"
}'
```

## Database Management Client

This is outside of the scope of this repo but I used `Robo 3T` on MacOS as a MongoDB Database Management Client.
