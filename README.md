# Instructions

* Source of practice from - https://www.railstutorial.org/book

### Commands to remember

* Create new Rails application


    rails _version.of.rails_ new hello_app --api --database=postgresql
 
 * Yarn install
 
 
    ### ERROR
    warning Integrity check: System parameters don't match
    error Integrity check failed
    error Found 1 errors.
    ========================================
      Your Yarn packages are out of date!
      Please run `yarn install --check-files` to update.
    ========================================
    To disable this check, please change `check_yarn_integrity`
    to `false` in your webpacker config file (config/webpacker.yml).
    
    ### SOLUTION
    # If you get above error run the bellow command as suggested
    yarn install --check-files
    
    
### Explanation

* Gemfile


    gem 'capybara', '>= 2.15'
This installs the latest version of the capybara gem (which is used in testing) as long as it’s greater than or equal to version 2.15—even if it’s, say, version 7.2.

The second method looks like this:

    gem 'rails', '~> 6.0.3'
This installs the gem rails as long as it’s version 6.0.3 or newer but not 6.1 or newer. In other words, the >= notation always installs the latest gem, whereas the ~> 6.0.3 notation will install 6.0.4 (if available) but not 6.1.0.10
