require 'html-proofer'

task :test do
  sh "bundle exec jekyll build"
  HTMLProofer.check_directory("./_site",{alt_ignore:[/.*/],allow_hash_href:true}).run
end