# Rails Devise JWT Auth for API Only Mode


## Usage

1. Clone the repository to your local machine
2. Use ruby 3.2.0
3. Run `bundle install`
4. Run `rails db:create db:migrate`
5. Create user in Rails console  User.create(email: "foo@bar.com", password: "password")
6. Run `rails s` to start your api server on port 4000
7. Test out your [API using Postman](https://www.postman.com/orange-capsule-983544/workspace/rails-jwt)
   
 Endpoints:
 GET     http://localhost:4000/current_user   get info about user if you have valid JWT (use key 'Authorization')
 POST    http://localhost:4000/login          to login and get JWT (use keys 'email' and 'password')
 DELETE  http://localhost:4000/logout         to logout and destroy JWT (use key 'Authorization')
