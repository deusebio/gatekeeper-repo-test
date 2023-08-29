# Gatekeeper Test Repo

## Overview

This is a simple repository to be used for performing End-to-End tests on the [Discourse Gatekeeper]() Github Action, which enables sync between docs folder for charms and Discourse topics. 

This repository collects some Github Actions workflows to tests and make sure that Discourse Gatekeeper behaves as it should. The following workflows are currently implemented:

* **Pulling Tests (scheduled)** that simulates the workflow that would appear when community contribution are integrated in GitHub, also simulating when conflicts arise between Discourse and Github. *This tests only interacts with pre-existing topics in Discourse.* 
* **Pushing Tests (manually dispatched)** that simulates the workflow that would appear when non-conflicting content is pushed to Discourse. *This tests creates and deletes pages on Discourse, as part of the tests, so use it wisely to avoid creating too much cluttered content in Discourse*. 
