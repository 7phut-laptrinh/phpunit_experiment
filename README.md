# PHPUnit experimental project

Requires:
 - PHP installed in local machine
 - composer installed in local machine

## Run test

### Run all test cases
- Clone this project
- Install dependencies
```
composer install
```

Note: If you add more classes or change the class name, you have to re-generate the `autoload` file by running: `composer dump-autoload`

- Run test

On MacOS or Linux:

```
composer test_unix
```

On Windows:

```
composer test_win
```

### Run a specific test case
- Run as following command:
```
./vendor/bin/phpunit <filename> 

e.g 
./vendor/bin/phpunit test/00_hello_phpunit/HelloPHPUnitTest.php 
```

## Code structure

- All production code is put in folder `src` 

  - Each case will have a separate folder (e.g 00_hello_phpunit, ...)
  - In each folder, File `main.js` is where the code in that folder is used as examples.
    - You can run those files by command: `php -f <file_name>`
    - E.g: `php -f src/02_test_double/GameServer/main.php`
  
- All test code is put in folder `test`

## Reference documents

- [Juan Treminio's blog](https://jtreminio.com/blog/unit-testing-tutorial-part-v-mock-methods-and-overriding-constructors/)
- [PHPUnit manual](https://phpunit.readthedocs.io/en/9.1/index.html) 

Indeed, PHPUnit munual lacks many documentations, Juan Treminio's notes give us many more information about mocking objects, I own him a big thanks.

## Contact

- Email: 7phut.laptrinh@gmail.com
- Facebook page: https://www.facebook.com/nhungdongcodevui/
- Website: https://nhungdongcodevui.com/
