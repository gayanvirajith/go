require 'rake'

desc 'Preview the site with Jekyll'
task :preview do
    sh "jekyll serve --watch --drafts --baseurl '' --config _config.yml,_config-dev.yml"
end

desc 'Search site and print specific deprecation warnings'
task :check do 
    sh "jekyll doctor"
end

desc 'Git merge master branch changes to gh-pages;'
task :gh do
	git checkout gh-pages;
	git merge master;
	git push origin gh-pages;
	git checkout master;
end