```
$ cd /tmp

$ git clone https://github.com/matthewrudy/bundler2-heroku-example.git

Cloning into 'bundler2-heroku-example'...
remote: Enumerating objects: 94, done.
remote: Counting objects: 100% (94/94), done.
remote: Compressing objects: 100% (74/74), done.
remote: Total 94 (delta 5), reused 94 (delta 5), pack-reused 0
Unpacking objects: 100% (94/94), done.



$ cd bundler2-heroku-example

$ heroku create

Creating app... done, ⬢ infinite-sea-66853
https://infinite-sea-66853.herokuapp.com/ | https://git.heroku.com/infinite-sea-66853.git



$ heroku buildpacks:set https://github.com/bundler/heroku-buildpack-bundler2.git

git Buildpack set. Next release on infinite-sea-66853 will use https://github.com/bundler/heroku-buildpack-bundler2.git.
Run git push heroku master to create a new release using this buildpack.



$ git push heroku master

Enumerating objects: 94, done.
Counting objects: 100% (94/94), done.
Delta compression using up to 4 threads
Compressing objects: 100% (79/79), done.
Writing objects: 100% (94/94), 25.98 KiB | 1023.00 KiB/s, done.
Total 94 (delta 5), reused 0 (delta 0)
remote: Compressing source files... done.
remote: Building source:
remote:
remote: -----> Ruby app detected
remote: -----> Compiling Ruby/Rails
remote: -----> Using Ruby version: ruby-2.6.0
remote: -----> Installing dependencies using bundler 2.0.1
remote:        Running: bundle install --without development:test --path vendor/bundle --binstubs vendor/bundle/bin -j4 --deployment
remote:        The dependency tzinfo-data (>= 0) will be unused by any of the platforms Bundler is installing for. Bundler is installing for ruby but the dependency is only for x86-mingw32, x86-mswin32, x64-mingw32, java. To add those platforms to the bundle, run `bundle lock --add-platform x86-mingw32 x86-mswin32 x64-mingw32 java`.
remote:        Fetching gem metadata from https://rubygems.org/.........
remote:        Fetching rake 12.3.2
remote:        Installing rake 12.3.2
remote:        Fetching concurrent-ruby 1.1.4
remote:        Fetching thread_safe 0.3.6
remote:        Fetching minitest 5.11.3
remote:        Installing minitest 5.11.3
remote:        Installing thread_safe 0.3.6
remote:        Installing concurrent-ruby 1.1.4
remote:        Fetching builder 3.2.3
remote:        Installing builder 3.2.3
remote:        Fetching erubi 1.8.0
remote:        Fetching mini_portile2 2.4.0
remote:        Installing mini_portile2 2.4.0
remote:        Installing erubi 1.8.0
remote:        Fetching crass 1.0.4
remote:        Installing crass 1.0.4
remote:        Fetching rack 2.0.6
remote:        Installing rack 2.0.6
remote:        Fetching nio4r 2.3.1
remote:        Fetching websocket-extensions 0.1.3
remote:        Installing nio4r 2.3.1 with native extensions
remote:        Installing websocket-extensions 0.1.3
remote:        Fetching mini_mime 1.0.1
remote:        Installing mini_mime 1.0.1
remote:        Fetching arel 9.0.0
remote:        Installing arel 9.0.0
remote:        Fetching mimemagic 0.3.3
remote:        Installing mimemagic 0.3.3
remote:        Fetching msgpack 1.2.6
remote:        Installing msgpack 1.2.6 with native extensions
remote:        Using bundler 2.0.1
remote:        Fetching coffee-script-source 1.12.2
remote:        Installing coffee-script-source 1.12.2
remote:        Fetching execjs 2.7.0
remote:        Installing execjs 2.7.0
remote:        Fetching method_source 0.9.2
remote:        Installing method_source 0.9.2
remote:        Fetching thor 0.20.3
remote:        Installing thor 0.20.3
remote:        Fetching ffi 1.10.0
remote:        Installing ffi 1.10.0 with native extensions
remote:        Fetching multi_json 1.13.1
remote:        Installing multi_json 1.13.1
remote:        Fetching pg 1.1.3
remote:        Installing pg 1.1.3 with native extensions
remote:        Fetching puma 3.12.0
remote:        Installing puma 3.12.0 with native extensions
remote:        Fetching rb-fsevent 0.10.3
remote:        Installing rb-fsevent 0.10.3
remote:        Fetching tilt 2.0.9
remote:        Installing tilt 2.0.9
remote:        Fetching turbolinks-source 5.2.0
remote:        Installing turbolinks-source 5.2.0
remote:        Fetching tzinfo 1.2.5
remote:        Installing tzinfo 1.2.5
remote:        Fetching nokogiri 1.10.0
remote:        Installing nokogiri 1.10.0 with native extensions
remote:        Fetching i18n 1.5.1
remote:        Installing i18n 1.5.1
remote:        Fetching websocket-driver 0.7.0
remote:        Installing websocket-driver 0.7.0 with native extensions
remote:        Fetching mail 2.7.1
remote:        Installing mail 2.7.1
remote:        Fetching rack-test 1.1.0
remote:        Installing rack-test 1.1.0
remote:        Fetching sprockets 3.7.2
remote:        Installing sprockets 3.7.2
remote:        Fetching marcel 0.3.3
remote:        Installing marcel 0.3.3
remote:        Fetching coffee-script 2.4.1
remote:        Installing coffee-script 2.4.1
remote:        Fetching uglifier 4.1.20
remote:        Installing uglifier 4.1.20
remote:        Fetching bootsnap 1.3.2
remote:        Installing bootsnap 1.3.2 with native extensions
remote:        Fetching rb-inotify 0.10.0
remote:        Installing rb-inotify 0.10.0
remote:        Fetching turbolinks 5.2.0
remote:        Installing turbolinks 5.2.0
remote:        Fetching activesupport 5.2.2
remote:        Installing activesupport 5.2.2
remote:        Fetching loofah 2.2.3
remote:        Fetching sass-listen 4.0.0
remote:        Installing loofah 2.2.3
remote:        Installing sass-listen 4.0.0
remote:        Fetching globalid 0.4.1
remote:        Fetching rails-dom-testing 2.0.3
remote:        Installing globalid 0.4.1
remote:        Installing rails-dom-testing 2.0.3
remote:        Fetching activemodel 5.2.2
remote:        Fetching jbuilder 2.8.0
remote:        Installing activemodel 5.2.2
remote:        Installing jbuilder 2.8.0
remote:        Fetching sass 3.7.3
remote:        Installing sass 3.7.3
remote:        Fetching rails-html-sanitizer 1.0.4
remote:        Installing rails-html-sanitizer 1.0.4
remote:        Fetching activejob 5.2.2
remote:        Installing activejob 5.2.2
remote:        Fetching activerecord 5.2.2
remote:        Fetching actionview 5.2.2
remote:        Installing actionview 5.2.2
remote:        Installing activerecord 5.2.2
remote:        Fetching actionpack 5.2.2
remote:        Installing actionpack 5.2.2
remote:        Fetching actioncable 5.2.2
remote:        Fetching activestorage 5.2.2
remote:        Fetching actionmailer 5.2.2
remote:        Installing actionmailer 5.2.2
remote:        Installing activestorage 5.2.2
remote:        Installing actioncable 5.2.2
remote:        Fetching railties 5.2.2
remote:        Fetching sprockets-rails 3.2.1
remote:        Installing sprockets-rails 3.2.1
remote:        Installing railties 5.2.2
remote:        Fetching coffee-rails 4.2.2
remote:        Fetching sass-rails 5.0.7
remote:        Fetching rails 5.2.2
remote:        Installing coffee-rails 4.2.2
remote:        Installing sass-rails 5.0.7
remote:        Installing rails 5.2.2
remote:        Bundle complete! 18 Gemfile dependencies, 61 gems now installed.
remote:        Gems in the groups development and test were not installed.
remote:        Bundled gems are installed into `./vendor/bundle`
remote:        Post-install message from i18n:
remote:
remote:        HEADS UP! i18n 1.1 changed fallbacks to exclude default locale.
remote:        But that may break your application.
remote:
remote:        Please check your Rails app for 'config.i18n.fallbacks = true'.
remote:        If you're using I18n (>= 1.1.0) and Rails (< 5.2.2), this should be
remote:        'config.i18n.fallbacks = [I18n.default_locale]'.
remote:        If not, fallbacks will be broken in your app by I18n 1.1.x.
remote:
remote:        For more info see:
remote:        https://github.com/svenfuchs/i18n/releases/tag/v1.1.0
remote:
remote:        Post-install message from sass:
remote:
remote:        Ruby Sass is deprecated and will be unmaintained as of 26 March 2019.
remote:
remote:        * If you use Sass as a command-line tool, we recommend using Dart Sass, the new
remote:          primary implementation: https://sass-lang.com/install
remote:
remote:        * If you use Sass as a plug-in for a Ruby web framework, we recommend using the
remote:          sassc gem: https://github.com/sass/sassc-ruby#readme
remote:
remote:        * For more details, please refer to the Sass blog:
remote:          http://sass.logdown.com/posts/7081811
remote:
remote:        Bundle completed (43.00s)
remote:        Cleaning up the bundler cache.
remote: -----> Installing node-v8.10.0-linux-x64
remote: -----> Detecting rake tasks
remote: -----> Preparing app for Rails asset pipeline
remote:        Running: rake assets:precompile
remote:        Yarn executable was not detected in the system.
remote:        Download Yarn at https://yarnpkg.com/en/docs/install
remote:        I, [2019-01-08T14:12:16.887237 #1272]  INFO -- : Writing /tmp/build_8243231091dcbb562d191c0df1ad33fa/public/assets/application-fbacdb1bf716e4009d7c179c0cd2cb3f42014fed637c57e6aee3cc9e583ad94c.js
remote:        I, [2019-01-08T14:12:16.887735 #1272]  INFO -- : Writing /tmp/build_8243231091dcbb562d191c0df1ad33fa/public/assets/application-fbacdb1bf716e4009d7c179c0cd2cb3f42014fed637c57e6aee3cc9e583ad94c.js.gz
remote:        I, [2019-01-08T14:12:16.893437 #1272]  INFO -- : Writing /tmp/build_8243231091dcbb562d191c0df1ad33fa/public/assets/application-e3b0c44298fc1c149afbf4c8996fb92427ae41e4649b934ca495991b7852b855.css
remote:        I, [2019-01-08T14:12:16.893564 #1272]  INFO -- : Writing /tmp/build_8243231091dcbb562d191c0df1ad33fa/public/assets/application-e3b0c44298fc1c149afbf4c8996fb92427ae41e4649b934ca495991b7852b855.css.gz
remote:        Asset precompilation completed (3.46s)
remote:        Cleaning assets
remote:        Running: rake assets:clean
remote: -----> Detecting rails configuration
remote:
remote: ###### WARNING:
remote:
remote:        You set your `config.active_storage.service` to :local in production.
remote:        If you are uploading files to this app, they will not persist after the app
remote:        is restarted, on one-off dynos, or if the app has multiple dynos.
remote:        Heroku applications have an ephemeral file system. To
remote:        persist uploaded files, please use a service such as S3 and update your Rails
remote:        configuration.
remote:
remote:        For more information can be found in this article:
remote:          https://devcenter.heroku.com/articles/active-storage-on-heroku
remote:
remote:
remote: ###### WARNING:
remote:
remote:        We detected that some binary dependencies required to
remote:        use all the preview features of Active Storage are not
remote:        present on this system.
remote:
remote:        For more information please see:
remote:          https://devcenter.heroku.com/articles/active-storage-on-heroku
remote:
remote:
remote:
remote: -----> Discovering process types
remote:        Procfile declares types     -> release, web
remote:        Default types for buildpack -> console, rake
remote:
remote: -----> Compressing...
remote:        Done: 41.7M
remote: -----> Launching...
remote:  !     Release command declared: this new release will not be available until the command succeeds.
remote:        Released v6
remote:        https://infinite-sea-66853.herokuapp.com/ deployed to Heroku
remote:
remote: Verifying deploy... done.
remote: Running release command...
remote:
remote: Bundler::LockfileError: You must use Bundler 2 or greater with this lockfile.
remote:   /app/vendor/ruby-2.6.0/lib/ruby/2.6.0/bundler/lockfile_parser.rb:108:in `warn_for_outdated_bundler_version'
remote:   /app/vendor/ruby-2.6.0/lib/ruby/2.6.0/bundler/lockfile_parser.rb:95:in `initialize'
remote:   /app/vendor/ruby-2.6.0/lib/ruby/2.6.0/bundler/definition.rb:83:in `new'
remote:   /app/vendor/ruby-2.6.0/lib/ruby/2.6.0/bundler/definition.rb:83:in `initialize'
remote:   /app/vendor/ruby-2.6.0/lib/ruby/2.6.0/bundler/dsl.rb:234:in `new'
remote:   /app/vendor/ruby-2.6.0/lib/ruby/2.6.0/bundler/dsl.rb:234:in `to_definition'
remote:   /app/vendor/ruby-2.6.0/lib/ruby/2.6.0/bundler/dsl.rb:13:in `evaluate'
remote:   /app/vendor/ruby-2.6.0/lib/ruby/2.6.0/bundler/definition.rb:34:in `build'
remote:   /app/vendor/ruby-2.6.0/lib/ruby/2.6.0/bundler.rb:135:in `definition'
remote:   /app/vendor/ruby-2.6.0/lib/ruby/2.6.0/bundler.rb:101:in `setup'
remote:   /app/vendor/ruby-2.6.0/lib/ruby/2.6.0/bundler/setup.rb:20:in `<top (required)>'
remote:   /app/vendor/ruby-2.6.0/lib/ruby/2.6.0/rubygems/core_ext/kernel_require.rb:54:in `require'
remote:   /app/vendor/ruby-2.6.0/lib/ruby/2.6.0/rubygems/core_ext/kernel_require.rb:54:in `require'
remote: bundler: failed to load command: rails (/app/vendor/bundle/ruby/2.6.0/bin/rails)
remote: Waiting for release..... failed.
To https://git.heroku.com/infinite-sea-66853.git
 * [new branch]      master -> master
```
