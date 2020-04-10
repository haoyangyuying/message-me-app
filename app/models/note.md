### initial commit

### add root and login routes
chatroom_controller.rb: add index method
index.html.erb: add root route page template
new.html.erb: login page
routes.rb: add root, and get 'login'

### add semantic UI as front end framework
application.js: require jquery, require semantic-ui
custom.css.scss: @import "semantic-ui"
gemfile: gem 'semantic-ui-sass', gem 'jquery-rails'

### add navigation menu
application.html.erb: add menu bar

### add dropdown and nav paritial
_navigation.html.erb: items
application.html.erb: 'layouts/navigation'
application.js: after turbolink load to load dropdown

### add favicon
application.html.erb: favicon_link_tag

### Build Homepage
custom.css.scsss: chatbox style
index.html.erb: ui two column grid

### Complete homepage
index.html.erb: ui small feed / ui header

### Add login page
Link_to 'Log in', login_path, class: "item"
new.html.erb: ui center aligned large header

### add root route link to navigation
<%= link_to "Chatroom", root_path, class: "item" %>

### add users resource
db: migrate,schema.rb,seeds.rb
test: user_test.rb

### add uniqueness constraint to username
user.rb: username, presence: true, length: { minium: 3, maxmum: 15 }

### Add message resource
app/models: belongs_to :user
validates :body, presence: true


