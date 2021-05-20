# NodeJS Challenge 02
The second challenge of Rocketseat's Ignite Node JS bootcamp. This time I further enhanced the last challenge with middlewares.


### What have I learned?
I'm creating a series of blog posts showcasing my routine and achievements on the road to become a Fullstack Developer. If you're interested in checking it out, I would love to welcome you into [my blog](https://alansiqueira.com).


# Goals

### checksExistsUserAccount
This middleware should retrieve a *username* from the *request header* and validate if it already exists. If it exists, the *user* should be registered in the request.

### checksCreateTodosUserAvailability
This middleware should receive the *user* from the *request* (as registered before) and check the following conditions:
- Should validate if a user is *Pro*;
- If it's a free user, should validate if there are already 10 *todos* or more created.
- Should allow pro users through;
- Should stop free users that have 10 todos or more;

### checksTodoExists
This middleware retrieves the *username* from the request header and a todo *id* from the request params. You should validate that given id is valid (is a uuid) and that it is contained inside the user's todos list. 

After those validations, the given *todo* should be passed through the *request* along with the given *user*.


### findUserById
Just like the checkExistsUserAccount, this middleware should validate the existance of a user. But this time, it will receive a *id* through *request params*. If it finds a user that matches that criteria, it should be stored in the request as usual.
