rails generate scaffold Apartment address:string price:float description:text image_url:string --no-test-framework

Fix:
form.html.erb --> replace the top line with:
"form_for(post) do |form|"

post.rb in models --> inherit from ActiveRecord::Base
