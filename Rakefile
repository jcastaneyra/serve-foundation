desc "Upgrade Foundation to latest version (you need to update the Gemfile first)"
task :upgrade do
  system("bundle install")
  system("bundle exec compass create public/ -r zurb-foundation --using foundation --force")
  system("mv public/sass/* sass/")
  system("rm -Rf public/sass")
  system("rm public/config.rb")
  system("bundle exec html2haml public/index.html views/index.html.haml")
  system("rm public/index.html")
end

task :default => :upgrade