## Working with `Rails new` defaults

Rails has several default options you can use when creating a new app. For example, if you want to skip bundle install, skip default test units, and set your default database to psql, you can run the following: 

```bash
$ rails new new_options -B -T -d postgresql
```

Although you will want to run `bundle install` to run your new application, one use case for skipping it is if you want to have gems installed in a specific gemset that is created after generating the Rails app. 

Skipping Rail's default test suite is popular if you'd like to use another test framework such as Rspec. Similarly, defaulting to postgressql or another database is a good way to default to the db you would like to use. 

If you'd like to have your defaults used for all future generated Rails apps, you can configured the default Rails command to always include those options by putting them in your `.railsrc` file. 