# hebrews Installation Steps

Step 1: Install Composer
- follow this guide https://www.thecodedeveloper.com/install-composer-windows-xampp/#:~:text=1)%20First%20go%20to%20Download,Click%20the%20Next%20button.

Step 2: Install Nodejs
- https://nodejs.org/en/

Step 3: Add/enable php extensions to php.ini of XAMPP
-intl, pdo_mysql, mbstring, exif, pcntl, bcmath, zip, gd
- you can follow this guide on how to enable extensions in xampp https://stackoverflow.com/questions/33869521/how-can-i-enable-php-extension-intl

Step 4: Add Repo to your local
    1. Downlaod or clone repository https://github.com/nathanielgb/hebrews
    2. extract the file and put it in htdocs of xampp

Step 5: Installation of project
    1. Goto terminal and cd into the directory of project
    2. In the root directory of the project, find file with filename ".env.example". make a new file with filename ".env" and copy content of ".env.example" into ".env"
    3. In .env file change the ff. fields according to your mysql credentials in myphpadmin of xampp and save
        DB_USERNAME=root
        DB_PASSWORD=mypassword
    4. Next, run the ff. commands in the terminal in order
        1. composer install
        2. npm install
        3. php artisan key:generate
        4. php artisan migrate (for database tables)
        5. php artisan db:seed (for initial values of tables)
        * use the ff as guide
            -https://devmarketer.io/learn/setup-laravel-project-cloned-github-com/
            -https://www.youtube.com/watch?v=H3PV5_TweKU

Step 6: Run command this command in terminal to run the project "php artisan serve"

For importing of inventories and menus use this files as proper format of excel sheet
https://drive.google.com/drive/folders/1ztzDj-ulsKCjfedxtL5kDMTWXl-XXF4W?usp=share_link

