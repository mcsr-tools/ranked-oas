# MCSR API OpenAPI Specification
This is an **Unofficial** OpenAPI specificaton for [MSCR's API](https://docs.mcsrranked.com)


## TODOs
- Ensure all nullable fields are documented
- Add statistics for `/users/{identifier}`
- Some dictionaries that are ranked/casual key-specific are not implemented yet
- Make `/live` status an enum
- Fix descriptions and add missing descriptions to certian ref objects
- Verify common tools support OpenAPI `3.1.0` and upgrade to that, since certain features (like descriptions on ref objects) are not supported in `3.0.0`
- Make some note or enforcement of the rate limit of "500 requests per 10 minutes unless otherwise specified"


### MCSR API TODOs
Some additional information is also needed about the API to implement parts of the spec
- Connection object for user info (i think they should be strings)
- Which requests can return 400/401
- Which response objects are nullable (e.g. seasonResult is listed as nullable but seasonResults isn't)
- Valid values for third party connection keys
- Objects like MatchSeed have nullable strings but empty arrays (not nullable for some reason)
- `Any?` type is not clear, what should it be?
- What is `roleType`?
- What is the default `status` for `/users/{identifier}/live`