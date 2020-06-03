Role Name
=========

A role for testing function testing of the internal workings


TEST-ROLE
--------------

* `test-role/defaults/main.yml` has all the test data for exercising the parsers
* `test-role/tests/test.yml` has example tasks of parsing the example router output output and asserting that the values are correct
* `test-role/parsers/show_xxxxxxxxx.yml` are in a format for the parse_cli filter plugin and named for the show command that
    generated the output.
    

Running tests
-------------

From the test-role directory.

```
ansible-playbook tests/test.yml -i test/inventory
```
