> Add spec alias for "require spec helper" and first test.
> They took out assets group in Rails 4.
> Outside in testing 
> Add Capybara DSL 
> All Rspec tests have to have spec in the name.
> I really should make my own generator.
> Tmux changing the crap thing.
> Start rails on alternate port in Guard.
> Controller structure: Home has its own controller (no model, show action only). Dashboard has its own controller (no model, show action only).
> Controllers need not be connected to models.
> render text: "DO the text". That's the right syntax.
> Setting up devise via migration, then the initializers, then the views in the folder,
> First time to do the seeding thing on Rails. JESUS CHRIST DO NOT FORGET THE PRIMARY KEY.
> Testing thing sa thoughtbot: CodeClimate, simplecov if env["coverage"]. Requires: rspec/autorun, rspec/rails, paperclip/matchers, webmock/rspec, clearance/testing
> FakeStripeRunnner, FakeGithubRunner, Capybara js driver = webkit. Mocks: Mocha.
> FactoryGirl+Faker: Require the Faker (or FFaker) at top. Also, FFaker still uses Faker in the factories themselves.
> No need to restart guard when FG has been modified.
> Iba yung `user_session_path` sa `new_user_session_path`
> Important thing for devise:

    <%= form_for(:user, :url => session_path(:user)) do |f| %>
      <%= f.text_field :email %>
      <%= f.password_field :password %>
      <%= f.check_box :remember_me %>
      <%= f.label :remember_me %>
      <%= f.submit 'Sign in' %>
      <%= link_to "Forgot your password?", new_password_path(:user) %>
    <% end %>

 
2-25
> High voltage for a cleaner static pages controller/route action.
> Padding library is in neat. neat has a gem too
> Email kasi, hindi email address!!!
> Rspec support modules need to be included in the spec_helper file.
> structure of sign in helpers and factory I sort of know now
> Don't make nested namespaces and attempt to include all of them, that doesn't make sense lol.
> Don't forget the `it` block, you end up with weird `undefined method get` and `undefined method response`.
> If you don't put the controller spec in the spec/controllers directory, you will need to specify `:type => controller` in the describe block at the start.
> Always work in the feature branch and merge from main. If you are on main then you have to delete the feature branch again.
> Though it is expected that you have to try `expect` syntax in Rspec, you can still use the `should` syntax and the `shoulda_matchers` gem. You don't need to always use the "convention".
