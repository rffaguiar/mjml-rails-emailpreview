## How to run
1. `git clone git@github.com:rffaguiar/mjml-rails-emailpreview.git`
2. `bundle install`
3. `npm install -g mjml@^2.0` -g is optional
4. `rake db:migrate`
5. go to the folder and start the server `rails s`
6. go to `http://localhost:3000/emails` and click welcome email
7. you can also open console with `rails c` and run `UserMailer.welcome_email(User.new).deliver_now` to see the email with letter opener gem.

Go to `app/views/user_mailer/welcome_email.mjml` and see that we are using MJML markup with partials and ruby variables.

Rails email building in a easier way.
