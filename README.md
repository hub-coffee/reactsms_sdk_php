# react-sms-sdk-php

ReactSMS SDK for PHP 


## Example Send Message

    $AUTH_KEY = "rs_xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx";
    $API_KEY = "rs_xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx";
    $SERVICE_KEY = "xxxxxx";

    $reactsms = new Reactsms($AUTH_KEY, $API_KEY, $SERVICE_KEY);

    $response = $reactsms->send_message("Just a test", [["zip_code" => "+225", "number" => "0758187266"]]);
    print($response);


## Example Balance Checking

    $AUTH_KEY = "rs_xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx";
    $API_KEY = "rs_xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx";

    $reactsms = new Reactsms($AUTH_KEY, $API_KEY);

    $response = $reactsms->balance();
    print($response);


## Example Create service

    $AUTH_KEY = "rs_xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx";
    $API_KEY = "rs_xxxxxxxxxxxxxxxxxxxxxxxxxxxxxxxx";

    $reactsms = new Reactsms($AUTH_KEY, $API_KEY, $SERVICE_KEY);

    $response = $reactsms->create_service($service_name, $quota_sms, $active_quota, $description);
    print($response);



