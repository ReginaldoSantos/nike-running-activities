# nike-running-activities

Just a place to store my nike running activities.


## Running The Script

1. Open Chrome Browser (it should work in Firefox, Safari and Opera as well);

2. Open DevTools (F12 on Chrome);

3. On DevTools, go to *"Network"* tab;

4. Paste this URL in the Browser Address Bar [Nike Running App Login URL](https://unite.nike.com/s3/unite/mobile.html?androidSDKVersion=3.1.0&corsoverride=https://unite.nike.com&uxid=com.nike.sport.running.droid.3.8&locale=en_US&backendEnvironment=identity&view=login&clientId=WLr1eIG5JSNNcBJM3npVa6L76MK8OBTt&facebookAppId=84697719333&wechatAppId=wxde7d0246cfaf32f7);

5. Back to DevTools search for a request like this: https://unite.nike.com.br/login?

6. If it is the right one, on inner tab "Preview" you should find an "access_token" like below:

![image](/images/devtools_access_token.png)

The important part for us is the "access_token" value.

7. For now on, just refer to this as an environment variable "BEARER_TOKEN";

8. Go to terminal and run the *nike_running_fetch_all.sh* script as below:

```
sh nike_running_fetch_all.sh $BEARER_TOKEN
```

