require 'rubygems'
require 'markaby'

desc "run rake build to do everythang!"
task :default => [:remove_old_posts, :remove_old_site, :jekyll] do
end

desc "discard the contents of _posts, we will be rebuilding each time"
task :remove_old_posts do
  puts "Remove old posts"
  system("rm -rf _posts/*")
end

desc "discard the contents of _site, remove old files and cruft"
task :remove_old_site do
  puts "Remove old site"
  system("rm -rf _site/*")
end

desc "run jekyll"
task :jekyll do
  puts "Run jekyll"
  system("jekyll")
end

desc "run jekyll --server"
task :server do
  puts "Run jekyll w/ server"
  system("jekyll --server")
end
