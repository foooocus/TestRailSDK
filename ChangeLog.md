##  Changes between 0.8 and 0.9

There are no breaking API changes. The new features introduced are all backward compatible. Please let the project team know if this turns out not to be the case (open an issue on github)

 * (issue #9) Adding retry for 429 response
 * (issue #9) `suite_mode` added to Project entity
 * (issue #9) `description` added to Section entity
 * (issue #9) `completed_on`, `is_completed`, `is_baseline`, `is_master` added to TestSuite entity
 * `add_run` endpoint support - allows you to create new TestRun entities
 * `add_plan` endpoint support - allows you to create new TestPlan entities
 * `add_milestone` endpoint support - allows you to create new Milestones
 * `get_result` and `get_results` endpoint support. You can now query TestResults!
 * `get_user`, `get_user_by_email`, and `get_users` endpoing support - allows you to query users
 * addTestPlanEntry() method for TestRun/Milestone support
 * added (private) `postRESTBodyReturn` method to TestRailService to make POST abstraction easier
 * added generics support to same, improved testability of the code, and added some integration tests
 * Made getEntityList and getEntitySingle protected instead of private (to facilitate customizations)
 * Fixed a bug which obscured the root cause of a connection error with the TestRail server. Now the stack trace will actually print correctly)
 * (issue #5) Downgraded to Java 1.6 at a user's request
 * Made integration tests query for a "Sandbox" project in which to perform the destructive tests
 * (issue #8) Added support for those with local TestRail instance to be able to do so (previous version only supported hosted installations, e.g. "https://mycompany.testrail.com/")
 * Unit tests updated accordingly (but not 100% coverage yet)
 
 