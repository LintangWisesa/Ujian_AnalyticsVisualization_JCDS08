![Lintang_Purwadhika](https://static.wixstatic.com/media/2e6af2_f69a4271c3534ae1869a7ed63e278b2b~mv2.png/v1/fill/w_246,h_39,al_c,usm_0.66_1.00_0.01/2e6af2_f69a4271c3534ae1869a7ed63e278b2b~mv2.png)

## Import retrowheels.sql to your local MySQL

1. Download & place this _retrowheels.sql_ on your local MySQL ```bin``` directory, for example: ```C:\Program Files\MySQL\MySQL Server 8.0\bin```.

2. Open terminal/cmd as an administrator, then go to MySQL ```bin``` directory.
    
    ```bash
    $ cd C:\Program Files\MySQL\MySQL Server 8.0\bin
    $ mysql -u username -p
    ```

3. Create database _retrowheels_, and exit.
    
    ```bash
    mysql> create database retrowheels;
    mysql> exit
    ```

4. Import _retrowheels.sql_ to _retrowheels_ database.

    ```bash
    $ mysql -u username -p -D retrowheels < retrowheels.sql
    $ mysql -u username -p
    
    mysql> show databases;
    mysql> use retrowheels
    ```

5. Enjoy!

<hr>

### *__#HappyCoding__* :relaxed:

#### Lintang Wisesa :love_letter: _lintangwisesa@ymail.com_

[Facebook](https://www.facebook.com/lintangbagus) | 
[Twitter](https://twitter.com/Lintang_Wisesa) |
[Google+](https://plus.google.com/u/0/+LintangWisesa1) |
[Youtube](https://www.youtube.com/user/lintangbagus) | 
:octocat: [GitHub](https://github.com/LintangWisesa) |
[Hackster](https://www.hackster.io/lintangwisesa)