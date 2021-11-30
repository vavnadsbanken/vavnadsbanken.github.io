To run
bundle exec jekyll serve

Add stuff to gemfile
bundle add <what to install>
bundle install <what to install>

Generate thumbnails
convert -define jpeg:size=200x200 ./images/2021-03-09-construction/construction1.jpg  -thumbnail 200x200^ -gravity center -extent 200x200  ./images/2021-03-09-construction/construction1-thumb.jpg
convert ./images/2021-03-09-construction/construction3.jpg  -resize 400x400 ./images/2021-03-09-construction/construction3-thumb.jpg