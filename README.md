# hw09-intro-to-rails

# URLS
1. /
2. /gifs
3. /gifs/23463-cats-jumping
1 passes to 2, 2 passes to 3

# Routers, controller#action, params, templates
1. displays the root for the site, controller#action = welcome#index, template = index.html.erb (plus any other sub templates for links)
2. displays a list of gifs, controller#action = gifs#index, template = default
3. displays a specific gif, controller#action = gifs#view, params = gif, template = view.html.erb (from the gif directory in 'app')

Three controllers exist for the application (at least)
-   1. application_controller.rb
-   2. welcome_controller.rb
-   3. gifs_controller.rb


The welcome and gifs controllers inherit from the application controller.
The param for /gifs/23463-cats-jumping should be @gif = params[:gif]

A layout is like a default template for the application or a set of classes. Whereas a template is a more specific erb file for rendering content. For example, the index page (welcome#index) will use the application's layout (application.html.erb) but it will also probably have a template file (index.html.erb) specific to the welcome controller.

