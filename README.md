## Without bundler

$ ruby -rubygems bin/test

/Users/david/.gems/gems/sequel-3.20.0/lib
/Users/david/.gems/gems/mysql-2.8.1/lib
/Users/david/.gems/gems/mysql-2.8.1/ext
/Library/Ruby/Site/1.8
/Library/Ruby/Site/1.8/powerpc-darwin10.4.0
/Library/Ruby/Site/1.8/universal-darwin10.4.0
/Library/Ruby/Site
/System/Library/Frameworks/Ruby.framework/Versions/1.8/usr/lib/ruby/vendor_ruby/1.8
/System/Library/Frameworks/Ruby.framework/Versions/1.8/usr/lib/ruby/vendor_ruby/1.8/universal-darwin10.4.0
/System/Library/Frameworks/Ruby.framework/Versions/1.8/usr/lib/ruby/vendor_ruby
/System/Library/Frameworks/Ruby.framework/Versions/1.8/usr/lib/ruby/1.8
/System/Library/Frameworks/Ruby.framework/Versions/1.8/usr/lib/ruby/1.8/powerpc-darwin10.4.0
/System/Library/Frameworks/Ruby.framework/Versions/1.8/usr/lib/ruby/1.8/universal-darwin10.4.0
.

[:products]

## With bundler

/Users/david/.bundle/gems/sequel-3.21.0/lib
/Users/david/.bundle/gems/mysql-2.8.1/lib
/Users/david/.bundle/gems/mysql-2.8.1/ext
/Users/david/.gems/gems/bundler-1.0.10/gems/bundler-1.0.10/lib
/Users/david/.gems/gems/bundler-1.0.10/lib
/Library/Ruby/Site/1.8
/Library/Ruby/Site/1.8/powerpc-darwin10.4.0
/Library/Ruby/Site/1.8/universal-darwin10.4.0
/Library/Ruby/Site
/System/Library/Frameworks/Ruby.framework/Versions/1.8/usr/lib/ruby/vendor_ruby/1.8
/System/Library/Frameworks/Ruby.framework/Versions/1.8/usr/lib/ruby/vendor_ruby/1.8/universal-darwin10.4.0
/System/Library/Frameworks/Ruby.framework/Versions/1.8/usr/lib/ruby/vendor_ruby
/System/Library/Frameworks/Ruby.framework/Versions/1.8/usr/lib/ruby/1.8
/System/Library/Frameworks/Ruby.framework/Versions/1.8/usr/lib/ruby/1.8/powerpc-darwin10.4.0
/System/Library/Frameworks/Ruby.framework/Versions/1.8/usr/lib/ruby/1.8/universal-darwin10.4.0
.


/Users/david/.bundle/gems/sequel-3.21.0/lib/sequel/adapters/mysql.rb:6: LoadError: require 'mysql' did not define Mysql::CLIENT_MULTI_RESULTS! (Sequel::AdapterNotFound)
  You are probably using the pure ruby mysql.rb driver,
  which Sequel does not support. You need to install
  the C based adapter, and make sure that the mysql.so
  file is loaded instead of the mysql.rb file.
        from /Users/david/.bundle/gems/sequel-3.21.0/lib/sequel/core.rb:249:in `k_require'
        from /Users/david/.bundle/gems/sequel-3.21.0/lib/sequel/core.rb:249:in `tsk_require'
        from /Users/david/.bundle/gems/sequel-3.21.0/lib/sequel/core.rb:72:in `check_requiring_thread'
        from /Users/david/.bundle/gems/sequel-3.21.0/lib/sequel/core.rb:69:in `synchronize'
        from /Users/david/.bundle/gems/sequel-3.21.0/lib/sequel/core.rb:69:in `check_requiring_thread'
        from /Users/david/.bundle/gems/sequel-3.21.0/lib/sequel/core.rb:249:in `tsk_require'
        from /Users/david/.bundle/gems/sequel-3.21.0/lib/sequel/database/connecting.rb:25:in `adapter_class'
        from /Users/david/.bundle/gems/sequel-3.21.0/lib/sequel/database/connecting.rb:54:in `connect'
        from /Users/david/.bundle/gems/sequel-3.21.0/lib/sequel/core.rb:119:in `connect'
        from bin/test:5
