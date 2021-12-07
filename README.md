# Client Project Template

## *See [Planning File](./planning.md) for current plans.*


## Rest API

### /v1/:campus/:cohort

*Access is restricted based on the cohorts of which the user has visibility based on github team visibility*

#### /repos

|Method|path|description|
|----|----|----|
|GET|`/`|Get all repos for the cohort|

#### /status

|Method|path|description|
|----|----|----|
|GET|`/`|Gets status for all published repos|


#### /events

|Method|path|description|
|----|----|----|
|GET|`/`|Get all events for the cohort|

#### Campus codes (enum)

|Campus code|Long Name|
|----|----|
|rfp|Remote Full Time Pacific|
|rfe|Remote Full Time Eastern|
|atx|Austin, TX|
|nye|New York, NY|
|den|Denver, CO|
|lax|Los Angeles, CA|
|sfo|San Francisco, CA|
|sjo|San Jose, CA|


#### External APIs

|Method|path|description|API doc Link|
|----|----|----|----|
|GET|`/repos/{owner}/{repo}/traffic/clones`|Get repository clones (requires push access)|[get clones](https://docs.github.com/en/rest/reference/repos#traffic)|
|GET|`/repos/{owner}/{repo}/hooks`|List repository webhooks|[get webhooks](https://docs.github.com/en/rest/reference/repos#webhooks)|
|GET|`/repos/{owner}/{repo}/pulls/{pull_number}`|Get a Pull Request|[get pull request](https://docs.github.com/en/rest/reference/pulls#get-a-pull-request)|
|GET|`/repos/{owner}/{repo}`|Get a repository|[Get a repository](https://docs.github.com/en/rest/reference/repos#get-a-repository)|
