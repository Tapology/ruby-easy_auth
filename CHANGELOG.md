### EasyAuth 0.3.4

* Moved `AuthenticatedController#attempt_to_authenticate` into
  `EasyAuthHelper` for general use.
### EasyAuth 0.3.3

* Remove gin index

### EasyAuth 0.3.2

* Redirect to `request.fullpath` after successful sign-in

### EasyAuth 0.3.1

* Remove dependent -> destroy inifinite loop

### EasyAuth 0.3.0

* Reverted array identities
* Updated Rails to ~> 4.0.0
* Identities are destroy dependent of parent
* Identities are always autosave
* Identities will require validation for parent to save
* Identities require presence of token
* Accounts accept nested attributes for identities
* SessionsController#create will rescue DoubleRenderErrors
