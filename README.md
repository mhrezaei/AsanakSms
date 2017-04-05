
package's home : [mhrezaei/asanak-sms](https://github.com/mhrezaei/AsanakSms/) 


----------


**Installation**:

Run below statements on your terminal :

STEP 1 : 

    composer require "mhrezaei/asanak-sms":"dev-master"
    
STEP 2 : Add `provider` and `facade` in config/app.php

    'providers' => [
      ...
      Asanak\Sms\AsanakSmsProvider::class, // <-- add this line at the end of provider array
    ],


    'aliases' => [
      ...
      'AsanakSms' => Asanak\Sms\Facade\AsanakSmsFacade::class, // <-- add this line at the end of aliases array
    ]

Step 3:  

    php artisan vendor:publish --tag=AsanakSmsTag --force

Configuration file is placed in config/asanak-sms.php , open it and enter your Asanak webservice config: