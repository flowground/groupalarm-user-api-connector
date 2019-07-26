# ![LOGO](logo.png) groupalarm User API **flow**ground Connector

## Description

A generated **flow**ground connector for the groupalarm User API API (version 1.16.1).

Generated from: https://app.groupalarm.com/api/v1<br/>
Generated at: 2019-07-26T13:59:37+03:00

## API Description

The user service implements all user functions for GroupAlarm.<br/>
<br/>
# Authentication<br/>
<br/>
<!-- ReDoc-Inject: <security-definitions> --><br/>

## Authorization

Supported authorization schemes:
- API Key
- API Key

## Actions

### Login
> Handles the user login and returns a user payload with JWT token<br/>

*Tags:* `auth`

### GetInvitationText
> Get the organization's saved invitation text configuration<br/>

*Tags:* `invitation-config`

### SetInvitationText
> Set the organization's invitation text configuration<br/>

*Tags:* `invitation-config`

### MFAIsActive
> Check if the current user has MFA enabled or not<br/>

*Tags:* `mfa`

### MFACreate
> Creates a new, disabled MFA config for the current user<br/>

*Tags:* `mfa`

### MFAEnable
> Enables a new MFA config for the current user<br/>

*Tags:* `mfa`

#### Input Parameters
* `code` - _required_ - current MFA code<br/>

### MFADisable
> Disables the MFA config for the current user<br/>

*Tags:* `mfa`

#### Input Parameters
* `code` - _required_ - current MFA code<br/>

### MFAGenerateBackupCodes
> Creates ten new, one-time-use backup codes<br/>

*Tags:* `mfa`

### Deletes the current user irreversibly.
> Can only be used after leaving all organizations.<br/>

*Tags:* `user`

### GetSettings
> Get the current user's saved settings or the default settings if none are found<br/>

*Tags:* `settings`

### StoreSettings
> Saves the current user's settings<br/>

*Tags:* `settings`

### GetUser
> Gets the complete user payload from the passed JWT token<br/>

*Tags:* `user`

### UpdateUser
> Updates the user profile<br/>

*Tags:* `user`

### InviteUser
> Invites an existing or new user to an organization and sends an invitation email to the passed address<br/>

*Tags:* `user`

### GetSpecificUser
> Returns a specific user with the passed api for organization members<br/>

*Tags:* `user`

#### Input Parameters
* `userID` - _required_ - ID of an user<br/>
* `organization` - _required_ - ID of the organization<br/>

### DeleteUserFromOrganization
> Removes a user from an organization<br/>

*Tags:* `user`

#### Input Parameters
* `userID` - _required_ - user by his ID<br/>
* `organizationID` - _required_ - organization by it's ID<br/>

### GetUsersInOrganization
> Returns all users from an organization<br/>

*Tags:* `users`

#### Input Parameters
* `organization` - _required_ - organization by it's ID<br/>

### AddUserAvailabilityChange
> Add a new availability change for the current user or update an existing one<br/>

*Tags:* `availability`

### GetUsersInOrganizationPagination
> Returns all users from an organization with pagination<br/>

*Tags:* `users`

#### Input Parameters
* `organization` - _required_ - organization by it's ID<br/>
* `limit` - _optional_ - max. amount of entries in list<br/>
* `offset` - _optional_ - amount of entries to skip<br/>

## License

**flow**ground :- Telekom iPaaS / groupalarm-user-api-connector<br/>
Copyright © 2019, [Deutsche Telekom AG](https://www.telekom.de)<br/>
contact: flowground@telekom.de

All files of this connector are licensed under the Apache 2.0 License. For details
see the file LICENSE on the toplevel directory.
