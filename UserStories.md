# User Stories

## Controlling

### Backend

* An Authority User must be able to register, login and log out from a Backend
* An Unprotected User should be able to register, login and log out from a Backend
* An Authority User must be able to maintain Unprotected User data (such as
    email, name, addresses).
* An Unprotected User should be able to maintain their own data.

General Idea:

The whole idea that I'm proposing here is that Unprotected Users don't need a
login/credential to be able to use the service. The usage of the service must
be completely hassle-free & password-free in order to be as easy and
non-invasive as possible. Logins for Unprotected Users SHOULD be possible to maintain their own data.

### Services

#### Dead Mans Switch

* An authority must be able to create, edit & delete a "dead mans switch
  service" for unprotected users
* A dead man's switch must appear as a button (or notification or similar) on the
    Unprotected User's device.
* A dead mans switch configuration must be initially confirmed on an Unprotected User's
    device.
* A dead man's switch has an interval; if the dead man's switch is not
    "pressed" during that interval the creating Authority User must receive a
    notification/warning.
* An Authority user must be able to discard such a warning.

#### "Communication Channel from Unprotected to Authority"

@omarsotillo feel free to sketch further ideas here


### Frontend

TBD: Also - how does a frontend to an Unprotected User look like?
