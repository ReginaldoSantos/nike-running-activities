# nike-running-activities

Just a place to store my nike running activities.


## Running The Script

1. Get into Nike web site from a web browser;

2. Open DevTools (F12 on Chrome);

3. On DevTools, go to Network tab;

4. Log into you Nike Running App Account;

5. Back to DevTools search for a request like this: https://unite.nike.com.br/login

6. If it is the right one, on inner tab "Response" you should find an "access_token" like below:

```
eyJhbGciOiJSUzI1NiIsImtpZCI6ImFlYmJkMWMyLTNjNDUtNDM5NS04MGMzLTA2NjYifQ==.eyJ0cnVzdCI6MTAwLCJpYXQiOjE1OTY0Nzg2NjYsImV4cCI6MTU5NjQ4MTc2MSwiaXNzIjoib2F1dGgyYWNjIiwianRpIjoiMTZmYjgyNGQtYzcyNy00YmIzLTlhODctMjllZjA1Mjc1NjY2IiwibGF0IjoxNTk2NDc4NjY2LCJhdWQiOiJjb20ubmlrZS5kaWdpdGFsIiwic3ViIjoiY29tLm5pa2UuY29tbWVyY2UubmlrZWRvdGNvbS53ZWIiLCJzYnQiOiJuaWtlOmFwcCIsInNjcCI6WyJuaWtlLmRpZ2l0YWwiXSwicHJuIjoiMTQyNTk0NzUxOTYiLCJwcnQiOiJuaWtlOnBsdXMifQ==.0xNlEYJTMlMJAN9Jv_z7FIcSyBlaxCO7C1ayMwWfnK4VoZNtnn2ZGpYlmAhI9tbDlxR90FX_B9uFmuIWuW6KLbGlH4YMlSlIncu7oM99fPAIhiR0BC0x6gF3FnJ83utSKs6ITKTKYK9HCGkKV_GCNfvaOVOW8yp_grXGHkMMhHv8yndeyHVUPOreaH9H9u41lxfMf2-55XlHjrI-BJuuGgnA53TjNlVYthi1UBlCuVa4jwCmA7xXcoUBgeU1WMoMo0w7eOv44t6_5XRtQqj1hxWtK0eiVfMJoyhksg9mZWDYCt_4YPpjN9YKwonaWIfan-ZRS5Y0GFttg-_F2ySPKQ
```

7. For now on, just refer to this as an environment variable "BEARER_TOKEN";

8. Go to terminal and run the *nike_running_fetch_all.sh* script as below:

```
sh nike_running_fetch_all.sh $BEARER_TOKEN
```

