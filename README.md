# MCSR Ranked REST API OAS

> [!NOTE]
> Unaffiliated with MCSR Ranked. Some info might be missing or inaccurate.

Community maintained **unofficial** [MCSR Ranked REST API](https://docs.mcsrranked.com) OAS. Useful for generating types, creating SDKs, documentation, etc. See [openapi.tools](https://openapi.tools) for more information.

View [examples](https://github.com/mcsr-tools/ranked-oas/wiki/Examples) on how to generate useful code for your programming language of choice.

## TODOs

- Ensure all nullable fields are documented
- Add statistics for `/users/{identifier}`
- Some dictionaries that are ranked/casual key-specific are not implemented yet
- Make `/live` status an enum
- Fix descriptions and add missing descriptions to certian ref objects
- Verify common tools support OpenAPI `3.1.0` and upgrade to that, since certain features (like descriptions on ref objects) are not supported in `3.0.0`

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
