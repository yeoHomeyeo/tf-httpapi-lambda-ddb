# Commands to invoke api
```bash
# Add movie
INVOKE_URL=https://xxxxxxx.amazonaws.com
curl \
  -X PUT \
  -H "Content-Type: application/json" \
  -d '{"year": "2013", "title": "The Amazing Spider"}' \
  ${INVOKE_URL}/topmovies

# Get movie for a particular year
curl ${INVOKE_URL}/topmovies/2013

# Get listing
curl ${INVOKE_URL}/topmovies

# Delete movie for a particular year
curl -X DELETE ${INVOKE_URL}/topmovies/2013
```


----------------------------------------------------------------------------------------------------------------
Fork the repository https://github.com/slim-sandbox/tf-httpapi-lambda-ddb
Be sure to uncheck “Copy the main branch only”
Clone the repository from your account
Change the branch of the local repository to solution. For avoidance of doubt, run the below commands in WSL/ Terminal similar to what is shown in the screenshot:
git clone https://github.com/slim-sandbox/tf-httpapi-lambda-ddb.git
cd tf-httpapi-lambda-ddb
git checkout solution


Deploy the resources
Execute`./send_request.sh` script multiple times (i.e. 3-5 times)


