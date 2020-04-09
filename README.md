## Objects

<dl>
<dt><a href="#vitals">vitals</a> : <code>object</code></dt>
<dd></dd>
<dt><a href="#utils">utils</a> : <code>object</code></dt>
<dd></dd>
</dl>

<a name="vitals"></a>

## vitals : <code>object</code>
<a name="vitals.AnonymousUser"></a>

### vitals.AnonymousUser
<a name="vitals.AnonymousUser.Client"></a>

#### AnonymousUser.Client(apiDomain, webServiceControlToken, apiToken, clientInfo)
<details>

| Param | Type |
| --- | --- |
| apiDomain | <code>string</code> | 
| webServiceControlToken | <code>string</code> | 
| apiToken | <code>string</code> | 
| clientInfo | <code>string</code> | 

</details><a name="vitals.AnonymousUser.Client.Create"></a>

##### Client.Create(userInformation)
<details>

| Param | Type |
| --- | --- |
| userInformation | <code>object</code> | 

</details><a name="vitals.AnonymousUser.Client.GetOrCreate"></a>

##### Client.GetOrCreate(userInformation)
<details>

| Param | Type |
| --- | --- |
| userInformation | <code>object</code> | 

</details><a name="vitals.AnonymousUser.Client.AnonymousUserExists"></a>

##### Client.AnonymousUserExists(anonymousUserExistsDetail)
<details>

| Param | Type |
| --- | --- |
| anonymousUserExistsDetail | <code>object</code> | 

</details><a name="vitals.AnonymousUser.Client.GetAnonymousUserDetails"></a>

##### Client.GetAnonymousUserDetails(anonymousUserTokenDetail)
<details>

| Param | Type |
| --- | --- |
| anonymousUserTokenDetail | <code>object</code> | 

</details><a name="vitals.AnonymousUser.Client.SaveAttributes"></a>

##### Client.SaveAttributes(anonymousUserTokenDetail, userAttributes)
<details>

| Param | Type |
| --- | --- |
| anonymousUserTokenDetail | <code>object</code> | 
| userAttributes | <code>object</code> | 

</details><a name="vitals.AnonymousUser.Client.GetAttributes"></a>

##### Client.GetAttributes(anonymousUserTokenDetail, userAttribute)
<details>

| Param | Type |
| --- | --- |
| anonymousUserTokenDetail | <code>object</code> | 
| userAttribute | <code>object</code> | 

</details><a name="vitals.Authentication"></a>

### vitals.Authentication
<a name="vitals.Authentication.Client"></a>

#### Authentication.Client(apiDomain, webServiceControlToken, apiToken, clientInfo)
<details>

| Param | Type |
| --- | --- |
| apiDomain | <code>string</code> | 
| webServiceControlToken | <code>string</code> | 
| apiToken | <code>string</code> | 
| clientInfo | <code>string</code> | 

</details><a name="vitals.Authentication.Client.CreateAccount"></a>

##### Client.CreateAccount(userInformation)
<details>

| Param | Type |
| --- | --- |
| userInformation | <code>object</code> | 

</details><a name="vitals.Authentication.Client.LoginAccount"></a>

##### Client.LoginAccount(AnonymousUserTokenDetail, AccountDetails)
<details>

| Param | Type |
| --- | --- |
| AnonymousUserTokenDetail | <code>object</code> | 
| AccountDetails | <code>object</code> | 

</details><a name="vitals.Authentication.Client.IsLoggedIn"></a>

##### Client.IsLoggedIn(AnonymousUserTokenDetail, AuthorizationToken)
<details>

| Param | Type |
| --- | --- |
| AnonymousUserTokenDetail | <code>object</code> | 
| AuthorizationToken | <code>object</code> | 

</details><a name="vitals.Authentication.Client.LogoutAccount"></a>

##### Client.LogoutAccount(AnonymousUserTokenDetail, AuthorizationToken)
<details>

| Param | Type |
| --- | --- |
| AnonymousUserTokenDetail | <code>object</code> | 
| AuthorizationToken | <code>object</code> | 

</details><a name="vitals.Authentication.Client.ForgotAccountPassword"></a>

##### Client.ForgotAccountPassword(AnonymousUserTokenDetail, ForgotAccountPasswordDetail)
<details>

| Param | Type |
| --- | --- |
| AnonymousUserTokenDetail | <code>object</code> | 
| ForgotAccountPasswordDetail | <code>object</code> | 

</details><a name="vitals.Authentication.Client.ValidateAccountPasswordResetToken"></a>

##### Client.ValidateAccountPasswordResetToken(AnonymousUserTokenDetail, ValidatePasswordResetTokenDetail)
<details>

| Param | Type |
| --- | --- |
| AnonymousUserTokenDetail | <code>object</code> | 
| ValidatePasswordResetTokenDetail | <code>object</code> | 

</details><a name="vitals.Authentication.Client.ResetAccountPassword"></a>

##### Client.ResetAccountPassword(AnonymousUserTokenDetail, PasswordResetTokenDetail)
<details>

| Param | Type |
| --- | --- |
| AnonymousUserTokenDetail | <code>object</code> | 
| PasswordResetTokenDetail | <code>object</code> | 

</details><a name="vitals.Authentication.Client.UpdateAccount"></a>

##### Client.UpdateAccount(AnonymousUserTokenDetail, authorizationToken, UpdateAccountDetail)
<details>

| Param | Type |
| --- | --- |
| AnonymousUserTokenDetail | <code>object</code> | 
| authorizationToken | <code>object</code> | 
| UpdateAccountDetail | <code>object</code> | 

</details><a name="vitals.Authentication.Client.ValidateAccount"></a>

##### Client.ValidateAccount(AnonymousUserTokenDetail, ValidateAccountDetail)
<details>

| Param | Type |
| --- | --- |
| AnonymousUserTokenDetail | <code>object</code> | 
| ValidateAccountDetail | <code>object</code> | 

</details><a name="vitals.DeviceManagement"></a>

### vitals.DeviceManagement
<a name="vitals.DeviceManagement.Client"></a>

#### DeviceManagement.Client(apiDomain, webServiceControlToken, apiToken, clientInfo)
<details>

| Param | Type |
| --- | --- |
| apiDomain | <code>string</code> | 
| webServiceControlToken | <code>string</code> | 
| apiToken | <code>string</code> | 
| clientInfo | <code>string</code> | 

</details><a name="vitals.DeviceManagement.Client.AppleDeviceLog"></a>

##### Client.AppleDeviceLog(DeviceLogs)
<details>

| Param | Type |
| --- | --- |
| DeviceLogs | <code>object</code> | 

</details><a name="vitals.DeviceManagement.Client.AppleGetPass"></a>

##### Client.AppleGetPass(PassDetail)
<details>

| Param | Type |
| --- | --- |
| PassDetail | <code>object</code> | 

</details><a name="vitals.DeviceManagement.Client.AppleRegisterPass"></a>

##### Client.AppleRegisterPass(RegisterPassDetail)
<details>

| Param | Type |
| --- | --- |
| RegisterPassDetail | <code>object</code> | 

</details><a name="vitals.DeviceManagement.Client.AppleUnregisterPass"></a>

##### Client.AppleUnregisterPass(UnregisterPassDetail)
<details>

| Param | Type |
| --- | --- |
| UnregisterPassDetail | <code>object</code> | 

</details><a name="vitals.DeviceManagement.Client.GetDevicePasses"></a>

##### Client.GetDevicePasses(RegisteredPassDetail)
<details>

| Param | Type |
| --- | --- |
| RegisteredPassDetail | <code>object</code> | 

</details><a name="vitals.FATPAdmin"></a>

### vitals.FATPAdmin
<a name="vitals.FATPAdmin.Client"></a>

#### FATPAdmin.Client(apiDomain, webServiceControlToken, apiToken, clientInfo)
<details>

| Param | Type |
| --- | --- |
| apiDomain | <code>string</code> | 
| webServiceControlToken | <code>string</code> | 
| apiToken | <code>string</code> | 
| clientInfo | <code>string</code> | 

</details><a name="vitals.FATPAdmin.Client.GetAddresses"></a>

##### Client.GetAddresses(userTokenDetail)
<details>

| Param | Type |
| --- | --- |
| userTokenDetail | <code>object</code> | 

</details><a name="vitals.FATPAdmin.Client.AddAddresses"></a>

##### Client.AddAddresses(userTokenDetail, addAddressesRequest)
<details>

| Param | Type |
| --- | --- |
| userTokenDetail | <code>object</code> | 
| addAddressesRequest | <code>object</code> | 

</details><a name="vitals.FATPAdmin.Client.UpdateAddresses"></a>

##### Client.UpdateAddresses(userTokenDetail, updateAddressesRequest)
<details>

| Param | Type |
| --- | --- |
| userTokenDetail | <code>object</code> | 
| updateAddressesRequest | <code>object</code> | 

</details><a name="vitals.FATPAdmin.Client.DeleteAddresses"></a>

##### Client.DeleteAddresses(userTokenDetail, deleteAddressesRequest)
<details>

| Param | Type |
| --- | --- |
| userTokenDetail | <code>object</code> | 
| deleteAddressesRequest | <code>object</code> | 

</details><a name="vitals.FATPAdmin.Client.GenerateExpiringUserToken"></a>

##### Client.GenerateExpiringUserToken(userToken)
<details>

| Param | Type |
| --- | --- |
| userToken | <code>object</code> | 

</details><a name="vitals.HCPUser"></a>

### vitals.HCPUser
<a name="vitals.HCPUser.Client"></a>

#### HCPUser.Client(apiDomain, webServiceControlToken, apiToken, clientInfo)
<details>

| Param | Type |
| --- | --- |
| apiDomain | <code>string</code> | 
| webServiceControlToken | <code>string</code> | 
| apiToken | <code>string</code> | 
| clientInfo | <code>string</code> | 

</details><a name="vitals.HCPUser.Client.CreateHCP"></a>

##### Client.CreateHCP(anonymousUserTokenDetail, hcpUserDetail, registrationSubscriptionDetail, surveyDetail)
<details>

| Param | Type |
| --- | --- |
| anonymousUserTokenDetail | <code>object</code> | 
| hcpUserDetail | <code>object</code> | 
| registrationSubscriptionDetail | <code>object</code> | 
| surveyDetail | <code>object</code> | 

</details><a name="vitals.HCPUser.Client.UpdateHCP"></a>

##### Client.UpdateHCP(registrantUserTokenDetail, hcpUserUpdateDetail, registrationSubscriptionDetail, surveyDetail)
<details>

| Param | Type |
| --- | --- |
| registrantUserTokenDetail | <code>object</code> | 
| hcpUserUpdateDetail | <code>object</code> | 
| registrationSubscriptionDetail | <code>object</code> | 
| surveyDetail | <code>object</code> | 

</details><a name="vitals.HCPUser.Client.GetByToken"></a>

##### Client.GetByToken(registrantUserTokenDetail)
<details>

| Param | Type |
| --- | --- |
| registrantUserTokenDetail | <code>object</code> | 

</details><a name="vitals.HCPUser.Client.IsHCPIdentifierValid"></a>

##### Client.IsHCPIdentifierValid(hcpIdentifierDetail)
<details>

| Param | Type |
| --- | --- |
| hcpIdentifierDetail | <code>object</code> | 

</details><a name="vitals.HCPUser.Client.GetHCPByToken"></a>

##### Client.GetHCPByToken(registrantUserTokenDetail)
<details>

| Param | Type |
| --- | --- |
| registrantUserTokenDetail | <code>object</code> | 

</details><a name="vitals.HCPUser.Client.GetHCPTypeMappingList"></a>

##### Client.GetHCPTypeMappingList(vendorProfessionSpecialty)
<details>

| Param | Type |
| --- | --- |
| vendorProfessionSpecialty | <code>object</code> | 

</details><a name="vitals.RegisteredUser"></a>

### vitals.RegisteredUser
<a name="vitals.RegisteredUser.Client"></a>

#### RegisteredUser.Client(apiDomain, webServiceControlToken, apiToken, clientInfo)
<details>

| Param | Type |
| --- | --- |
| apiDomain | <code>string</code> | 
| webServiceControlToken | <code>string</code> | 
| apiToken | <code>string</code> | 
| clientInfo | <code>string</code> | 

</details><a name="vitals.RegisteredUser.Client.Create"></a>

##### Client.Create(anonymousUserTokenDetail, registrantDetail, subscriptionDetail)
<details>

| Param | Type |
| --- | --- |
| anonymousUserTokenDetail | <code>object</code> | 
| registrantDetail | <code>object</code> | 
| subscriptionDetail | <code>object</code> | 

</details><a name="vitals.RegisteredUser.Client.CreatePatient"></a>

##### Client.CreatePatient(anonymousUserTokenDetail, registrantDetail, registrationSubscriptionDetail, surveyDetail)
<details>

| Param | Type |
| --- | --- |
| anonymousUserTokenDetail | <code>object</code> | 
| registrantDetail | <code>object</code> | 
| registrationSubscriptionDetail | <code>object</code> | 
| surveyDetail | <code>object</code> | 

</details><a name="vitals.RegisteredUser.Client.Update"></a>

##### Client.Update(registrantUserTokenDetail, registrantDetail, subscriptionDetail)
<details>

| Param | Type |
| --- | --- |
| registrantUserTokenDetail | <code>object</code> | 
| registrantDetail | <code>object</code> | 
| subscriptionDetail | <code>object</code> | 

</details><a name="vitals.RegisteredUser.Client.GetByToken"></a>

##### Client.GetByToken(registrantUserTokenDetail)
<details>

| Param | Type |
| --- | --- |
| registrantUserTokenDetail | <code>object</code> | 

</details><a name="vitals.RegisteredUser.Client.GetByEmail"></a>

##### Client.GetByEmail(anonymousUserTokenDetail, emailDetail)
<details>

| Param | Type |
| --- | --- |
| anonymousUserTokenDetail | <code>object</code> | 
| emailDetail | <code>object</code> | 

</details><a name="vitals.RegisteredUser.Client.GetSavingsCards"></a>

##### Client.GetSavingsCards(registrantUserTokenDetail)
<details>

| Param | Type |
| --- | --- |
| registrantUserTokenDetail | <code>object</code> | 

</details><a name="vitals.RegisteredUser.Client.ManageSubscriptionsByToken"></a>

##### Client.ManageSubscriptionsByToken(registrantUserTokenDetail, subscriptionDetail)
<details>

| Param | Type |
| --- | --- |
| registrantUserTokenDetail | <code>object</code> | 
| subscriptionDetail | <code>object</code> | 

</details><a name="vitals.RegisteredUser.Client.SendEmail"></a>

##### Client.SendEmail(registrantUserTokenDetail, messageCode)
<details>

| Param | Type |
| --- | --- |
| registrantUserTokenDetail | <code>object</code> | 
| messageCode | <code>object</code> | 

</details><a name="vitals.RegisteredUser.Client.AddUserToMarketingProgram"></a>

##### Client.AddUserToMarketingProgram(registrantUserTokenDetail, programCode)
<details>

| Param | Type |
| --- | --- |
| registrantUserTokenDetail | <code>object</code> | 
| programCode | <code>object</code> | 

</details><a name="vitals.RegisteredUser.Client.UpdatePatient"></a>

##### Client.UpdatePatient(registrantUserTokenDetail, registrantDetail, registrationSubscriptionDetail, surveyDetail)
<details>

| Param | Type |
| --- | --- |
| registrantUserTokenDetail | <code>object</code> | 
| registrantDetail | <code>object</code> | 
| registrationSubscriptionDetail | <code>object</code> | 
| surveyDetail | <code>object</code> | 

</details><a name="vitals.RegisteredUser.Client.GetPatientByToken"></a>

##### Client.GetPatientByToken(registrantUserTokenDetail)
<details>

| Param | Type |
| --- | --- |
| registrantUserTokenDetail | <code>object</code> | 

</details><a name="vitals.Request"></a>

### vitals.Request
<a name="vitals.Request.Client"></a>

#### Request.Client(apiDomain, webServiceControlToken, apiToken, clientInfo)
<details>

| Param | Type |
| --- | --- |
| apiDomain | <code>string</code> | 
| webServiceControlToken | <code>string</code> | 
| apiToken | <code>string</code> | 
| clientInfo | <code>string</code> | 

</details><a name="vitals.Request.Client.RegisteredUserRequest"></a>

##### Client.RegisteredUserRequest(registrantUserTokenDetail, requestDetail)
<details>

| Param | Type |
| --- | --- |
| registrantUserTokenDetail | <code>object</code> | 
| requestDetail | <code>object</code> | 

</details><a name="vitals.Request.Client.AnonymousUserRequest"></a>

##### Client.AnonymousUserRequest(anonymousUserTokenDetail, requestDetail)
<details>

| Param | Type |
| --- | --- |
| anonymousUserTokenDetail | <code>object</code> | 
| requestDetail | <code>object</code> | 

</details><a name="vitals.Request.Client.GetClinicalTrial"></a>

##### Client.GetClinicalTrial()
<a name="vitals.SavingsCards"></a>

### vitals.SavingsCards
<a name="vitals.SavingsCards.Client"></a>

#### SavingsCards.Client(apiDomain, webServiceControlToken, apiToken, clientInfo)
<details>

| Param | Type |
| --- | --- |
| apiDomain | <code>string</code> | 
| webServiceControlToken | <code>string</code> | 
| apiToken | <code>string</code> | 
| clientInfo | <code>string</code> | 

</details><a name="vitals.SavingsCards.Client.CreateCard"></a>

##### Client.CreateCard(registrantUserTokenDetail, cardRegistrationDetail)
<details>

| Param | Type |
| --- | --- |
| registrantUserTokenDetail | <code>object</code> | 
| cardRegistrationDetail | <code>object</code> | 

</details><a name="vitals.SavingsCards.Client.RegisterCardForUser"></a>

##### Client.RegisterCardForUser(userTokenDetail, cardRegistrationDetail)
<details>

| Param | Type |
| --- | --- |
| userTokenDetail | <code>object</code> | 
| cardRegistrationDetail | <code>object</code> | 

</details><a name="vitals.SavingsCards.Client.ActivateCard"></a>

##### Client.ActivateCard(registrantUserTokenDetail, cardActivationDetail)
<details>

| Param | Type |
| --- | --- |
| registrantUserTokenDetail | <code>object</code> | 
| cardActivationDetail | <code>object</code> | 

</details><a name="vitals.SavingsCards.Client.ValidateCard"></a>

##### Client.ValidateCard(userTokenDetail, cardValidationDetail)
<details>

| Param | Type |
| --- | --- |
| userTokenDetail | <code>object</code> | 
| cardValidationDetail | <code>object</code> | 

</details><a name="vitals.SMS"></a>

### vitals.SMS
<a name="vitals.SMS.Client"></a>

#### SMS.Client(apiDomain, webServiceControlToken, apiToken, clientInfo)
<details>

| Param | Type |
| --- | --- |
| apiDomain | <code>string</code> | 
| webServiceControlToken | <code>string</code> | 
| apiToken | <code>string</code> | 
| clientInfo | <code>string</code> | 

</details><a name="vitals.SMS.Client.SendTriggeredSMS"></a>

##### Client.SendTriggeredSMS(userTokenDetail, mailingCode)
<details>

| Param | Type |
| --- | --- |
| userTokenDetail | <code>object</code> | 
| mailingCode | <code>object</code> | 

</details><a name="vitals.SMS.Client.UnsubscribeBySms"></a>

##### Client.UnsubscribeBySms(anonymousUserTokenDetail, unsubscribeRequest)
<details>

| Param | Type |
| --- | --- |
| anonymousUserTokenDetail | <code>object</code> | 
| unsubscribeRequest | <code>object</code> | 

</details><a name="vitals.Survey"></a>

### vitals.Survey
<a name="vitals.Survey.Client"></a>

#### Survey.Client(apiDomain, webServiceControlToken, apiToken, clientInfo)
<details>

| Param | Type |
| --- | --- |
| apiDomain | <code>string</code> | 
| webServiceControlToken | <code>string</code> | 
| apiToken | <code>string</code> | 
| clientInfo | <code>string</code> | 

</details><a name="vitals.Survey.Client.SaveRegisteredUserSurveyDetails"></a>

##### Client.SaveRegisteredUserSurveyDetails(registrantUserTokenDetail, surveyRequests)
<details>

| Param | Type |
| --- | --- |
| registrantUserTokenDetail | <code>object</code> | 
| surveyRequests | <code>object</code> | 

</details><a name="vitals.Survey.Client.GetRegisteredUserSurveyDetails"></a>

##### Client.GetRegisteredUserSurveyDetails(registrantUserTokenDetail, requestFilters)
<details>

| Param | Type |
| --- | --- |
| registrantUserTokenDetail | <code>object</code> | 
| requestFilters | <code>object</code> | 

</details><a name="vitals.Survey.Client.SaveUserSurveyDetails"></a>

##### Client.SaveUserSurveyDetails(userTokenDetail, surveyDetail)
<details>

| Param | Type |
| --- | --- |
| userTokenDetail | <code>object</code> | 
| surveyDetail | <code>object</code> | 

</details><a name="vitals.Survey.Client.GetUserSurveyDetails"></a>

##### Client.GetUserSurveyDetails(userTokenDetail, requestFilters)
<details>

| Param | Type |
| --- | --- |
| userTokenDetail | <code>object</code> | 
| requestFilters | <code>object</code> | 

</details><a name="vitals.User"></a>

### vitals.User
<a name="vitals.User.Client"></a>

#### User.Client(apiDomain, webServiceControlToken, apiToken, clientInfo)
<details>

| Param | Type |
| --- | --- |
| apiDomain | <code>string</code> | 
| webServiceControlToken | <code>string</code> | 
| apiToken | <code>string</code> | 
| clientInfo | <code>string</code> | 

</details><a name="vitals.User.Client.SaveUserAttributes"></a>

##### Client.SaveUserAttributes(userTokenDetail, userAttributeDetail)
<details>

| Param | Type |
| --- | --- |
| userTokenDetail | <code>object</code> | 
| userAttributeDetail | <code>object</code> | 

</details><a name="vitals.User.Client.GetUserAttributes"></a>

##### Client.GetUserAttributes(userTokenDetail, userAttributeFilter)
<details>

| Param | Type |
| --- | --- |
| userTokenDetail | <code>object</code> | 
| userAttributeFilter | <code>object</code> | 

</details><a name="vitals.User.Client.UnsubscribeByEmail"></a>

##### Client.UnsubscribeByEmail(anonymousUserTokenDetail, unsubscribeRequest)
<details>

| Param | Type |
| --- | --- |
| anonymousUserTokenDetail | <code>object</code> | 
| unsubscribeRequest | <code>object</code> | 

</details><a name="vitals.User.Client.SendTriggeredEmail"></a>

##### Client.SendTriggeredEmail(userTokenDetail, mailingCode)
<details>

| Param | Type |
| --- | --- |
| userTokenDetail | <code>object</code> | 
| mailingCode | <code>object</code> | 

</details><a name="vitals.User.Client.FindADoctor"></a>

##### Client.FindADoctor(userTokenDetail, findADoctorDetail)
<details>

| Param | Type |
| --- | --- |
| userTokenDetail | <code>object</code> | 
| findADoctorDetail | <code>object</code> | 

</details><a name="vitals.User.Client.GetPendingInviteRequestsByUserToken"></a>

##### Client.GetPendingInviteRequestsByUserToken(userTokenDetail, PendingInviteRequestUserTokenQuery)
<details>

| Param | Type |
| --- | --- |
| userTokenDetail | <code>object</code> | 
| PendingInviteRequestUserTokenQuery | <code>object</code> | 

</details><a name="vitals.User.Client.GetPendingInviteRequestsByToken"></a>

##### Client.GetPendingInviteRequestsByToken(userTokenDetail, pendingInviteRequestTokenQuery)
<details>

| Param | Type |
| --- | --- |
| userTokenDetail | <code>object</code> | 
| pendingInviteRequestTokenQuery | <code>object</code> | 

</details><a name="vitals.User.Client.InviteUser"></a>

##### Client.InviteUser(userTokenDetail, inviteUserDetail)
<details>

| Param | Type |
| --- | --- |
| userTokenDetail | <code>object</code> | 
| inviteUserDetail | <code>object</code> | 

</details><a name="vitals.User.Client.LinkUser"></a>

##### Client.LinkUser(userTokenDetail, userLinkDetail)
<details>

| Param | Type |
| --- | --- |
| userTokenDetail | <code>object</code> | 
| userLinkDetail | <code>object</code> | 

</details><a name="vitals.User.Client.UnlinkUser"></a>

##### Client.UnlinkUser(userTokenDetail, userLinkDetail)
<details>

| Param | Type |
| --- | --- |
| userTokenDetail | <code>object</code> | 
| userLinkDetail | <code>object</code> | 

</details><a name="vitals.User.Client.ListUserLink"></a>

##### Client.ListUserLink(UserTokenDetail, UserLinkType)
<details>

| Param | Type |
| --- | --- |
| UserTokenDetail | <code>object</code> | 
| UserLinkType | <code>object</code> | 

</details><a name="vitals.User.Client.ListUserLinkIndividual"></a>

##### Client.ListUserLinkIndividual(UserTokenDetail, UserLinkIndividualDetail)
<details>

| Param | Type |
| --- | --- |
| UserTokenDetail | <code>object</code> | 
| UserLinkIndividualDetail | <code>object</code> | 

</details><a name="vitals.User.Client.ZipLocationLookup"></a>

##### Client.ZipLocationLookup(UserTokenDetail, ZipLocationDetail)
<details>

| Param | Type |
| --- | --- |
| UserTokenDetail | <code>object</code> | 
| ZipLocationDetail | <code>object</code> | 

</details><a name="vitals.User.Client.GetCorrectedAddress"></a>

##### Client.GetCorrectedAddress(UserTokenDetail, getCorrectedAddressDetail)
<details>

| Param | Type |
| --- | --- |
| UserTokenDetail | <code>object</code> | 
| getCorrectedAddressDetail | <code>object</code> | 

</details><a name="vitals.User.Client.GetUserByExternalId"></a>

##### Client.GetUserByExternalId(ExternalIdDetail)
<details>

| Param | Type |
| --- | --- |
| ExternalIdDetail | <code>object</code> | 

</details><a name="vitals.User.Client.ManageSubscriptionsByUserToken"></a>

##### Client.ManageSubscriptionsByUserToken(userTokenDetail, subscriptionDetail)
<details>

| Param | Type |
| --- | --- |
| userTokenDetail | <code>object</code> | 
| subscriptionDetail | <code>object</code> | 

</details><a name="vitals.User.Client.CreateUserExternalIdMapping"></a>

##### Client.CreateUserExternalIdMapping(UserTokenDetail, ExternalIdDetail)
<details>

| Param | Type |
| --- | --- |
| UserTokenDetail | <code>object</code> | 
| ExternalIdDetail | <code>object</code> | 

</details><a name="vitals.User.Client.FindAClinicalTrialLocation"></a>

##### Client.FindAClinicalTrialLocation(UserTokenDetail, FindAClinicalTrialLocationDetail)
<details>

| Param | Type |
| --- | --- |
| UserTokenDetail | <code>object</code> | 
| FindAClinicalTrialLocationDetail | <code>object</code> | 

</details><a name="vitals.User.Client.GenerateExpiringUserToken"></a>

##### Client.GenerateExpiringUserToken(emailAddress)
<details>

| Param | Type |
| --- | --- |
| emailAddress | <code>object</code> | 

</details><a name="vitals.User.Client.GetByExpiringUserToken"></a>

##### Client.GetByExpiringUserToken(expiringUserTokenValue)
<details>

| Param | Type |
| --- | --- |
| expiringUserTokenValue | <code>object</code> | 

</details><a name="vitals.User.Client.SaveUserActivities"></a>

##### Client.SaveUserActivities(userTokenDetail, userActivityDetails)
<details>

| Param | Type |
| --- | --- |
| userTokenDetail | <code>object</code> | 
| userActivityDetails | <code>object</code> | 

</details><a name="vitals.Util"></a>

### vitals.Util
<a name="vitals.Util.Client"></a>

#### Util.Client(apiDomain, webServiceControlToken, apiToken, clientInfo)
<details>

| Param | Type |
| --- | --- |
| apiDomain | <code>string</code> | 
| webServiceControlToken | <code>string</code> | 
| apiToken | <code>string</code> | 
| clientInfo | <code>string</code> | 

</details><a name="vitals.Util.Client.ClearCache"></a>

##### Client.ClearCache()
<a name="vitals.Util.Client.LogApplicationMessage"></a>

##### Client.LogApplicationMessage(applicationLogDetail)
<details>

| Param | Type |
| --- | --- |
| applicationLogDetail | <code>object</code> | 

</details><a name="vitals.Util.Client.GetConfiguration"></a>

##### Client.GetConfiguration(configurationFilters)
<details>

| Param | Type |
| --- | --- |
| configurationFilters | <code>object</code> | 

</details><a name="vitals.Util.Client.SaveJSON"></a>

##### Client.SaveJSON(container, record)
<details>

| Param | Type |
| --- | --- |
| container | <code>object</code> | 
| record | <code>object</code> | 

</details><a name="utils"></a>

## utils : <code>object</code>
<a name="utils.VitalsError"></a>

### utils.VitalsError ⇐ <code>Error</code>
**Extends**: <code>Error</code>  
<a name="new_utils.VitalsError_new"></a>

#### new VitalsError(method, result)
Creates an instance of VitalsError.

<details>

| Param | Type |
| --- | --- |
| method | <code>\*</code> | 
| result | <code>\*</code> | 

</details>
