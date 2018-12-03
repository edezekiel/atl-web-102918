
## Today's Goals

* Project Pitches at 11:30 or 1pm, we'll come around
  * Be ready with:
  * user stories
  * a rough timeline with targets for each day
* Learn what sessions are
* Understand when use of sessions is appropriate

## Step by Step(ish) - Day 1

1. Brief tour of project.

2. Warmup! Factor out the repeated "Post.find" logic
  * Whiteboard exercise?

3. Let's make it so that anything added to Flash
   displays on any page!
  * I'm not gonna dive into layouts too much.
    * But there are readings up if you want to learn more. :)
  * Cool, this feature is great but .. uh .. how does it work?
    * View request/response in browser and curl.
  * I bet we could use this for *other things* 😎

4. Hmm, any user can edit or delete any post.
  * Let's add a login form (in a LoginController?)
  * What problem does login solve?
    * What is your experience of login forms?
    * What does persistent mean? Is it persistent?
    * What forms of persistent storage do we know?

5. Track `user_id` in the session.

6. Display the current user in the layout.
  * Cool! Tomorrow, we'll see how to store passwords
    better, conveniently access the user, and secure
    our different routes! 😍

---

## Step by Step - Day 2

7. Add links to the layout for Login/Logout and Signup.

8. The two most common things the server will want to do are figure out
   who is making the current request and making sure a user is logged in
   to be able to view certain pages. Let's add methods to help with that!
  * Talk about `helper_method`!

9. Protect appropriate methods with a `before_action`.

10. Our password storage practices are bogus. Let's do a little better with `bcrypt`!
  * (and [`has_secure_password`][hsp])

[hsp]: http://api.rubyonrails.org/classes/ActiveModel/SecurePassword/ClassMethods.html
