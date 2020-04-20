## Objects

<dl>
<dt><a href="#vitals">vitals</a> : <code>object</code></dt>
<dd><p>The unofficial client for VITALS JSON Api</p>
</dd>
<dt><a href="#utils">utils</a> : <code>object</code></dt>
<dd></dd>
</dl>

<a name="vitals"></a>

## vitals : <code>object</code>
The unofficial client for VITALS JSON Api

**Example**  
```js
const vitalsUtils = require('@klickinc/util-vitals-json');

const HCPUserClient = new vitalsUtils.AnonymousUser.Client('https://klick-rm-dev-ws.klick.com', webServiceControlToken, apiToken);

const userInformation = {
    ipAddress,
    userAgent,
    dataOriginCode,
    anonymousUserToken,
};

await HCPUserClientt.GetOrCreate(userInformation);
```
<a name="vitals.AnonymousUser"></a>

### vitals.AnonymousUser
**Properties**

| Name | Type |
| --- | --- |
| Client | [<code>Client</code>](#vitals.AnonymousUser.Client) | 
| Models | <code>vitals.AnonymousUser.Models</code> | 

<a name="vitals.AnonymousUser.Client"></a>

#### AnonymousUser.Client
<a name="new_vitals.AnonymousUser.Client_new"></a>

##### new Client(apiDomain, webServiceControlToken, apiToken, clientInfo)
<details><summary></summary>

| Param | Type |
| --- | --- |
| apiDomain | <code>string</code> | 
| webServiceControlToken | <code>string</code> | 
| apiToken | <code>string</code> | 
| clientInfo | <code>string</code> | 

</details><a name="vitals.AnonymousUser.Client.Create"></a>

##### Client.Create(userInformation)
<details><summary></summary>

| Param | Type |
| --- | --- |
| userInformation | <code>object</code> | 

</details><a name="vitals.AnonymousUser.Client.GetOrCreate"></a>

##### Client.GetOrCreate(userInformation)
<details><summary></summary>

| Param | Type |
| --- | --- |
| userInformation | <code>object</code> | 

</details><a name="vitals.AnonymousUser.Client.AnonymousUserExists"></a>

##### Client.AnonymousUserExists(anonymousUserExistsDetail)
<details><summary></summary>

| Param | Type |
| --- | --- |
| anonymousUserExistsDetail | <code>object</code> | 

</details><a name="vitals.AnonymousUser.Client.GetAnonymousUserDetails"></a>

##### Client.GetAnonymousUserDetails(anonymousUserTokenDetail)
<details><summary></summary>

| Param | Type |
| --- | --- |
| anonymousUserTokenDetail | <code>object</code> | 

</details><a name="vitals.AnonymousUser.Client.SaveAttributes"></a>

##### Client.SaveAttributes(anonymousUserTokenDetail, userAttributes)
<details><summary></summary>

| Param | Type |
| --- | --- |
| anonymousUserTokenDetail | <code>object</code> | 
| userAttributes | <code>object</code> | 

</details><a name="vitals.AnonymousUser.Client.GetAttributes"></a>

##### Client.GetAttributes(anonymousUserTokenDetail, userAttribute)
<details><summary></summary>

| Param | Type |
| --- | --- |
| anonymousUserTokenDetail | <code>object</code> | 
| userAttribute | <code>object</code> | 

</details><a name="vitals.Authentication"></a>

### vitals.Authentication
**Properties**

| Name | Type |
| --- | --- |
| Client | [<code>Client</code>](#vitals.Authentication.Client) | 
| Models | <code>vitals.Authentication.Models</code> | 

<a name="vitals.Authentication.Client"></a>

#### Authentication.Client
<a name="new_vitals.Authentication.Client_new"></a>

##### new Client(apiDomain, webServiceControlToken, apiToken, clientInfo)
<details><summary></summary>

| Param | Type |
| --- | --- |
| apiDomain | <code>string</code> | 
| webServiceControlToken | <code>string</code> | 
| apiToken | <code>string</code> | 
| clientInfo | <code>string</code> | 

</details><a name="vitals.Authentication.Client.CreateAccount"></a>

##### Client.CreateAccount(userInformation)
<details><summary></summary>

| Param | Type |
| --- | --- |
| userInformation | <code>object</code> | 

</details><a name="vitals.Authentication.Client.LoginAccount"></a>

##### Client.LoginAccount(AnonymousUserTokenDetail, AccountDetails)
<details><summary></summary>

| Param | Type |
| --- | --- |
| AnonymousUserTokenDetail | <code>object</code> | 
| AccountDetails | <code>object</code> | 

</details><a name="vitals.Authentication.Client.IsLoggedIn"></a>

##### Client.IsLoggedIn(AnonymousUserTokenDetail, AuthorizationToken)
<details><summary></summary>

| Param | Type |
| --- | --- |
| AnonymousUserTokenDetail | <code>object</code> | 
| AuthorizationToken | <code>object</code> | 

</details><a name="vitals.Authentication.Client.LogoutAccount"></a>

##### Client.LogoutAccount(AnonymousUserTokenDetail, AuthorizationToken)
<details><summary></summary>

| Param | Type |
| --- | --- |
| AnonymousUserTokenDetail | <code>object</code> | 
| AuthorizationToken | <code>object</code> | 

</details><a name="vitals.Authentication.Client.ForgotAccountPassword"></a>

##### Client.ForgotAccountPassword(AnonymousUserTokenDetail, ForgotAccountPasswordDetail)
<details><summary></summary>

| Param | Type |
| --- | --- |
| AnonymousUserTokenDetail | <code>object</code> | 
| ForgotAccountPasswordDetail | <code>object</code> | 

</details><a name="vitals.Authentication.Client.ValidateAccountPasswordResetToken"></a>

##### Client.ValidateAccountPasswordResetToken(AnonymousUserTokenDetail, ValidatePasswordResetTokenDetail)
<details><summary></summary>

| Param | Type |
| --- | --- |
| AnonymousUserTokenDetail | <code>object</code> | 
| ValidatePasswordResetTokenDetail | <code>object</code> | 

</details><a name="vitals.Authentication.Client.ResetAccountPassword"></a>

##### Client.ResetAccountPassword(AnonymousUserTokenDetail, PasswordResetTokenDetail)
<details><summary></summary>

| Param | Type |
| --- | --- |
| AnonymousUserTokenDetail | <code>object</code> | 
| PasswordResetTokenDetail | <code>object</code> | 

</details><a name="vitals.Authentication.Client.UpdateAccount"></a>

##### Client.UpdateAccount(AnonymousUserTokenDetail, authorizationToken, UpdateAccountDetail)
<details><summary></summary>

| Param | Type |
| --- | --- |
| AnonymousUserTokenDetail | <code>object</code> | 
| authorizationToken | <code>object</code> | 
| UpdateAccountDetail | <code>object</code> | 

</details><a name="vitals.Authentication.Client.ValidateAccount"></a>

##### Client.ValidateAccount(AnonymousUserTokenDetail, ValidateAccountDetail)
<details><summary></summary>

| Param | Type |
| --- | --- |
| AnonymousUserTokenDetail | <code>object</code> | 
| ValidateAccountDetail | <code>object</code> | 

</details><a name="vitals.DeviceManagement"></a>

### vitals.DeviceManagement
**Properties**

| Name | Type |
| --- | --- |
| Client | [<code>Client</code>](#vitals.DeviceManagement.Client) | 
| Models | <code>vitals.DeviceManagement.Models</code> | 

<a name="vitals.DeviceManagement.Client"></a>

#### DeviceManagement.Client
<a name="new_vitals.DeviceManagement.Client_new"></a>

##### new Client(apiDomain, webServiceControlToken, apiToken, clientInfo)
<details><summary></summary>

| Param | Type |
| --- | --- |
| apiDomain | <code>string</code> | 
| webServiceControlToken | <code>string</code> | 
| apiToken | <code>string</code> | 
| clientInfo | <code>string</code> | 

</details><a name="vitals.DeviceManagement.Client.AppleDeviceLog"></a>

##### Client.AppleDeviceLog(DeviceLogs)
<details><summary></summary>

| Param | Type |
| --- | --- |
| DeviceLogs | <code>object</code> | 

</details><a name="vitals.DeviceManagement.Client.AppleGetPass"></a>

##### Client.AppleGetPass(PassDetail)
<details><summary></summary>

| Param | Type |
| --- | --- |
| PassDetail | <code>object</code> | 

</details><a name="vitals.DeviceManagement.Client.AppleRegisterPass"></a>

##### Client.AppleRegisterPass(RegisterPassDetail)
<details><summary></summary>

| Param | Type |
| --- | --- |
| RegisterPassDetail | <code>object</code> | 

</details><a name="vitals.DeviceManagement.Client.AppleUnregisterPass"></a>

##### Client.AppleUnregisterPass(UnregisterPassDetail)
<details><summary></summary>

| Param | Type |
| --- | --- |
| UnregisterPassDetail | <code>object</code> | 

</details><a name="vitals.DeviceManagement.Client.GetDevicePasses"></a>

##### Client.GetDevicePasses(RegisteredPassDetail)
<details><summary></summary>

| Param | Type |
| --- | --- |
| RegisteredPassDetail | <code>object</code> | 

</details><a name="vitals.FATPAdmin"></a>

### vitals.FATPAdmin
**Properties**

| Name | Type |
| --- | --- |
| Client | [<code>Client</code>](#vitals.FATPAdmin.Client) | 
| Models | <code>vitals.FATPAdmin.Models</code> | 

<a name="vitals.FATPAdmin.Client"></a>

#### FATPAdmin.Client
<a name="new_vitals.FATPAdmin.Client_new"></a>

##### new Client(apiDomain, webServiceControlToken, apiToken, clientInfo)
<details><summary></summary>

| Param | Type |
| --- | --- |
| apiDomain | <code>string</code> | 
| webServiceControlToken | <code>string</code> | 
| apiToken | <code>string</code> | 
| clientInfo | <code>string</code> | 

</details><a name="vitals.FATPAdmin.Client.GetAddresses"></a>

##### Client.GetAddresses(userTokenDetail)
<details><summary></summary>

| Param | Type |
| --- | --- |
| userTokenDetail | <code>object</code> | 

</details><a name="vitals.FATPAdmin.Client.AddAddresses"></a>

##### Client.AddAddresses(userTokenDetail, addAddressesRequest)
<details><summary></summary>

| Param | Type |
| --- | --- |
| userTokenDetail | <code>object</code> | 
| addAddressesRequest | <code>object</code> | 

</details><a name="vitals.FATPAdmin.Client.UpdateAddresses"></a>

##### Client.UpdateAddresses(userTokenDetail, updateAddressesRequest)
<details><summary></summary>

| Param | Type |
| --- | --- |
| userTokenDetail | <code>object</code> | 
| updateAddressesRequest | <code>object</code> | 

</details><a name="vitals.FATPAdmin.Client.DeleteAddresses"></a>

##### Client.DeleteAddresses(userTokenDetail, deleteAddressesRequest)
<details><summary></summary>

| Param | Type |
| --- | --- |
| userTokenDetail | <code>object</code> | 
| deleteAddressesRequest | <code>object</code> | 

</details><a name="vitals.FATPAdmin.Client.GenerateExpiringUserToken"></a>

##### Client.GenerateExpiringUserToken(UserTokenDetail)
<details><summary></summary>

| Param | Type |
| --- | --- |
| UserTokenDetail | <code>object</code> | 

</details><a name="vitals.HCPUser"></a>

### vitals.HCPUser
**Properties**

| Name | Type |
| --- | --- |
| Client | [<code>Client</code>](#vitals.HCPUser.Client) | 
| Models | <code>vitals.HCPUser.Models</code> | 

<a name="vitals.HCPUser.Client"></a>

#### HCPUser.Client
<a name="new_vitals.HCPUser.Client_new"></a>

##### new Client(apiDomain, webServiceControlToken, apiToken, clientInfo)
<details><summary></summary>

| Param | Type |
| --- | --- |
| apiDomain | <code>string</code> | 
| webServiceControlToken | <code>string</code> | 
| apiToken | <code>string</code> | 
| clientInfo | <code>string</code> | 

</details><a name="vitals.HCPUser.Client.CreateHCP"></a>

##### Client.CreateHCP(anonymousUserTokenDetail, hcpUserDetail, registrationSubscriptionDetail, surveyDetail)
<details><summary></summary>

| Param | Type |
| --- | --- |
| anonymousUserTokenDetail | <code>object</code> | 
| hcpUserDetail | <code>object</code> | 
| registrationSubscriptionDetail | <code>object</code> | 
| surveyDetail | <code>object</code> | 

</details><a name="vitals.HCPUser.Client.UpdateHCP"></a>

##### Client.UpdateHCP(registrantUserTokenDetail, hcpUserUpdateDetail, registrationSubscriptionDetail, surveyDetail)
<details><summary></summary>

| Param | Type |
| --- | --- |
| registrantUserTokenDetail | <code>object</code> | 
| hcpUserUpdateDetail | <code>object</code> | 
| registrationSubscriptionDetail | <code>object</code> | 
| surveyDetail | <code>object</code> | 

</details><a name="vitals.HCPUser.Client.GetByToken"></a>

##### Client.GetByToken(registrantUserTokenDetail)
<details><summary></summary>

| Param | Type |
| --- | --- |
| registrantUserTokenDetail | <code>object</code> | 

</details><a name="vitals.HCPUser.Client.IsHCPIdentifierValid"></a>

##### Client.IsHCPIdentifierValid(hcpIdentifierDetail)
<details><summary></summary>

| Param | Type |
| --- | --- |
| hcpIdentifierDetail | <code>object</code> | 

</details><a name="vitals.HCPUser.Client.GetHCPByToken"></a>

##### Client.GetHCPByToken(registrantUserTokenDetail)
<details><summary></summary>

| Param | Type |
| --- | --- |
| registrantUserTokenDetail | <code>object</code> | 

</details><a name="vitals.HCPUser.Client.GetHCPTypeMappingList"></a>

##### Client.GetHCPTypeMappingList(vendorProfessionSpecialty)
<details><summary></summary>

| Param | Type |
| --- | --- |
| vendorProfessionSpecialty | <code>object</code> | 

</details><a name="vitals.RegisteredUser"></a>

### vitals.RegisteredUser
**Properties**

| Name | Type |
| --- | --- |
| Client | [<code>Client</code>](#vitals.RegisteredUser.Client) | 
| Models | <code>vitals.RegisteredUser.Models</code> | 

<a name="vitals.RegisteredUser.Client"></a>

#### RegisteredUser.Client
<a name="new_vitals.RegisteredUser.Client_new"></a>

##### new Client(apiDomain, webServiceControlToken, apiToken, clientInfo)
<details><summary></summary>

| Param | Type |
| --- | --- |
| apiDomain | <code>string</code> | 
| webServiceControlToken | <code>string</code> | 
| apiToken | <code>string</code> | 
| clientInfo | <code>string</code> | 

</details><a name="vitals.RegisteredUser.Client.Create"></a>

##### Client.Create(anonymousUserTokenDetail, registrantDetail, subscriptionDetail)
<details><summary></summary>

| Param | Type |
| --- | --- |
| anonymousUserTokenDetail | <code>object</code> | 
| registrantDetail | <code>object</code> | 
| subscriptionDetail | <code>object</code> | 

</details><a name="vitals.RegisteredUser.Client.CreatePatient"></a>

##### Client.CreatePatient(anonymousUserTokenDetail, registrantDetail, registrationSubscriptionDetail, surveyDetail)
<details><summary></summary>

| Param | Type |
| --- | --- |
| anonymousUserTokenDetail | <code>object</code> | 
| registrantDetail | <code>object</code> | 
| registrationSubscriptionDetail | <code>object</code> | 
| surveyDetail | <code>object</code> | 

</details><a name="vitals.RegisteredUser.Client.Update"></a>

##### Client.Update(registrantUserTokenDetail, registrantDetail, subscriptionDetail)
<details><summary></summary>

| Param | Type |
| --- | --- |
| registrantUserTokenDetail | <code>object</code> | 
| registrantDetail | <code>object</code> | 
| subscriptionDetail | <code>object</code> | 

</details><a name="vitals.RegisteredUser.Client.GetByToken"></a>

##### Client.GetByToken(registrantUserTokenDetail)
<details><summary></summary>

| Param | Type |
| --- | --- |
| registrantUserTokenDetail | <code>object</code> | 

</details><a name="vitals.RegisteredUser.Client.GetByEmail"></a>

##### Client.GetByEmail(anonymousUserTokenDetail, emailDetail)
<details><summary></summary>

| Param | Type |
| --- | --- |
| anonymousUserTokenDetail | <code>object</code> | 
| emailDetail | <code>object</code> | 

</details><a name="vitals.RegisteredUser.Client.GetSavingsCards"></a>

##### Client.GetSavingsCards(registrantUserTokenDetail)
<details><summary></summary>

| Param | Type |
| --- | --- |
| registrantUserTokenDetail | <code>object</code> | 

</details><a name="vitals.RegisteredUser.Client.ManageSubscriptionsByToken"></a>

##### Client.ManageSubscriptionsByToken(registrantUserTokenDetail, subscriptionDetail)
<details><summary></summary>

| Param | Type |
| --- | --- |
| registrantUserTokenDetail | <code>object</code> | 
| subscriptionDetail | <code>object</code> | 

</details><a name="vitals.RegisteredUser.Client.SendEmail"></a>

##### Client.SendEmail(registrantUserTokenDetail, messageCode)
<details><summary></summary>

| Param | Type |
| --- | --- |
| registrantUserTokenDetail | <code>object</code> | 
| messageCode | <code>object</code> | 

</details><a name="vitals.RegisteredUser.Client.AddUserToMarketingProgram"></a>

##### Client.AddUserToMarketingProgram(registrantUserTokenDetail, programCode)
<details><summary></summary>

| Param | Type |
| --- | --- |
| registrantUserTokenDetail | <code>object</code> | 
| programCode | <code>object</code> | 

</details><a name="vitals.RegisteredUser.Client.UpdatePatient"></a>

##### Client.UpdatePatient(registrantUserTokenDetail, registrantDetail, registrationSubscriptionDetail, surveyDetail)
<details><summary></summary>

| Param | Type |
| --- | --- |
| registrantUserTokenDetail | <code>object</code> | 
| registrantDetail | <code>object</code> | 
| registrationSubscriptionDetail | <code>object</code> | 
| surveyDetail | <code>object</code> | 

</details><a name="vitals.RegisteredUser.Client.GetPatientByToken"></a>

##### Client.GetPatientByToken(registrantUserTokenDetail)
<details><summary></summary>

| Param | Type |
| --- | --- |
| registrantUserTokenDetail | <code>object</code> | 

</details><a name="vitals.Request"></a>

### vitals.Request
**Properties**

| Name | Type |
| --- | --- |
| Client | [<code>Client</code>](#vitals.Request.Client) | 
| Models | <code>vitals.Request.Models</code> | 

<a name="vitals.Request.Client"></a>

#### Request.Client
<a name="new_vitals.Request.Client_new"></a>

##### new Client(apiDomain, webServiceControlToken, apiToken, clientInfo)
<details><summary></summary>

| Param | Type |
| --- | --- |
| apiDomain | <code>string</code> | 
| webServiceControlToken | <code>string</code> | 
| apiToken | <code>string</code> | 
| clientInfo | <code>string</code> | 

</details><a name="vitals.Request.Client.RegisteredUserRequest"></a>

##### Client.RegisteredUserRequest(registrantUserTokenDetail, requestDetail)
<details><summary></summary>

| Param | Type |
| --- | --- |
| registrantUserTokenDetail | <code>object</code> | 
| requestDetail | <code>object</code> | 

</details><a name="vitals.Request.Client.AnonymousUserRequest"></a>

##### Client.AnonymousUserRequest(anonymousUserTokenDetail, requestDetail)
<details><summary></summary>

| Param | Type |
| --- | --- |
| anonymousUserTokenDetail | <code>object</code> | 
| requestDetail | <code>object</code> | 

</details><a name="vitals.Request.Client.GetClinicalTrial"></a>

##### Client.GetClinicalTrial()
<a name="vitals.SavingsCards"></a>

### vitals.SavingsCards
**Properties**

| Name | Type |
| --- | --- |
| Client | [<code>Client</code>](#vitals.SavingsCards.Client) | 
| Models | <code>vitals.SavingsCards.Models</code> | 

<a name="vitals.SavingsCards.Client"></a>

#### SavingsCards.Client
<a name="new_vitals.SavingsCards.Client_new"></a>

##### new Client(apiDomain, webServiceControlToken, apiToken, clientInfo)
<details><summary></summary>

| Param | Type |
| --- | --- |
| apiDomain | <code>string</code> | 
| webServiceControlToken | <code>string</code> | 
| apiToken | <code>string</code> | 
| clientInfo | <code>string</code> | 

</details><a name="vitals.SavingsCards.Client.CreateCard"></a>

##### Client.CreateCard(registrantUserTokenDetail, cardRegistrationDetail)
<details><summary></summary>

| Param | Type |
| --- | --- |
| registrantUserTokenDetail | <code>object</code> | 
| cardRegistrationDetail | <code>object</code> | 

</details><a name="vitals.SavingsCards.Client.RegisterCardForUser"></a>

##### Client.RegisterCardForUser(userTokenDetail, cardRegistrationDetail)
<details><summary></summary>

| Param | Type |
| --- | --- |
| userTokenDetail | <code>object</code> | 
| cardRegistrationDetail | <code>object</code> | 

</details><a name="vitals.SavingsCards.Client.ActivateCard"></a>

##### Client.ActivateCard(registrantUserTokenDetail, cardActivationDetail)
<details><summary></summary>

| Param | Type |
| --- | --- |
| registrantUserTokenDetail | <code>object</code> | 
| cardActivationDetail | <code>object</code> | 

</details><a name="vitals.SavingsCards.Client.ValidateCard"></a>

##### Client.ValidateCard(userTokenDetail, cardValidationDetail)
<details><summary></summary>

| Param | Type |
| --- | --- |
| userTokenDetail | <code>object</code> | 
| cardValidationDetail | <code>object</code> | 

</details><a name="vitals.SMS"></a>

### vitals.SMS
**Properties**

| Name | Type |
| --- | --- |
| Client | [<code>Client</code>](#vitals.SMS.Client) | 
| Models | <code>vitals.SMS.Models</code> | 

<a name="vitals.SMS.Client"></a>

#### SMS.Client
<a name="new_vitals.SMS.Client_new"></a>

##### new Client(apiDomain, webServiceControlToken, apiToken, clientInfo)
<details><summary></summary>

| Param | Type |
| --- | --- |
| apiDomain | <code>string</code> | 
| webServiceControlToken | <code>string</code> | 
| apiToken | <code>string</code> | 
| clientInfo | <code>string</code> | 

</details><a name="vitals.SMS.Client.SendTriggeredSMS"></a>

##### Client.SendTriggeredSMS(userTokenDetail, mailingCode)
<details><summary></summary>

| Param | Type |
| --- | --- |
| userTokenDetail | <code>object</code> | 
| mailingCode | <code>object</code> | 

</details><a name="vitals.SMS.Client.UnsubscribeBySms"></a>

##### Client.UnsubscribeBySms(anonymousUserTokenDetail, unsubscribeRequest)
<details><summary></summary>

| Param | Type |
| --- | --- |
| anonymousUserTokenDetail | <code>object</code> | 
| unsubscribeRequest | <code>object</code> | 

</details><a name="vitals.Survey"></a>

### vitals.Survey
**Properties**

| Name | Type |
| --- | --- |
| Client | [<code>Client</code>](#vitals.Survey.Client) | 
| Models | <code>vitals.Survey.Models</code> | 

<a name="vitals.Survey.Client"></a>

#### Survey.Client
<a name="new_vitals.Survey.Client_new"></a>

##### new Client(apiDomain, webServiceControlToken, apiToken, clientInfo)
<details><summary></summary>

| Param | Type |
| --- | --- |
| apiDomain | <code>string</code> | 
| webServiceControlToken | <code>string</code> | 
| apiToken | <code>string</code> | 
| clientInfo | <code>string</code> | 

</details><a name="vitals.Survey.Client.SaveRegisteredUserSurveyDetails"></a>

##### Client.SaveRegisteredUserSurveyDetails(registrantUserTokenDetail, surveyRequests)
<details><summary></summary>

| Param | Type |
| --- | --- |
| registrantUserTokenDetail | <code>object</code> | 
| surveyRequests | <code>object</code> | 

</details><a name="vitals.Survey.Client.GetRegisteredUserSurveyDetails"></a>

##### Client.GetRegisteredUserSurveyDetails(registrantUserTokenDetail, requestFilters)
<details><summary></summary>

| Param | Type |
| --- | --- |
| registrantUserTokenDetail | <code>object</code> | 
| requestFilters | <code>object</code> | 

</details><a name="vitals.Survey.Client.SaveUserSurveyDetails"></a>

##### Client.SaveUserSurveyDetails(userTokenDetail, surveyDetail)
<details><summary></summary>

| Param | Type |
| --- | --- |
| userTokenDetail | <code>object</code> | 
| surveyDetail | <code>object</code> | 

</details><a name="vitals.Survey.Client.GetUserSurveyDetails"></a>

##### Client.GetUserSurveyDetails(userTokenDetail, requestFilters)
<details><summary></summary>

| Param | Type |
| --- | --- |
| userTokenDetail | <code>object</code> | 
| requestFilters | <code>object</code> | 

</details><a name="vitals.User"></a>

### vitals.User
**Properties**

| Name | Type |
| --- | --- |
| Client | [<code>Client</code>](#vitals.User.Client) | 
| Models | <code>vitals.User.Models</code> | 

<a name="vitals.User.Client"></a>

#### User.Client
<a name="new_vitals.User.Client_new"></a>

##### new Client(apiDomain, webServiceControlToken, apiToken, clientInfo)
<details><summary></summary>

| Param | Type |
| --- | --- |
| apiDomain | <code>string</code> | 
| webServiceControlToken | <code>string</code> | 
| apiToken | <code>string</code> | 
| clientInfo | <code>string</code> | 

</details><a name="vitals.User.Client.SaveUserAttributes"></a>

##### Client.SaveUserAttributes(userTokenDetail, userAttributeDetail)
<details><summary></summary>

| Param | Type |
| --- | --- |
| userTokenDetail | <code>object</code> | 
| userAttributeDetail | <code>object</code> | 

</details><a name="vitals.User.Client.GetUserAttributes"></a>

##### Client.GetUserAttributes(userTokenDetail, userAttributeFilter)
<details><summary></summary>

| Param | Type |
| --- | --- |
| userTokenDetail | <code>object</code> | 
| userAttributeFilter | <code>object</code> | 

</details><a name="vitals.User.Client.UnsubscribeByEmail"></a>

##### Client.UnsubscribeByEmail(anonymousUserTokenDetail, unsubscribeRequest)
<details><summary></summary>

| Param | Type |
| --- | --- |
| anonymousUserTokenDetail | <code>object</code> | 
| unsubscribeRequest | <code>object</code> | 

</details><a name="vitals.User.Client.SendTriggeredEmail"></a>

##### Client.SendTriggeredEmail(userTokenDetail, mailingCode)
<details><summary></summary>

| Param | Type |
| --- | --- |
| userTokenDetail | <code>object</code> | 
| mailingCode | <code>object</code> | 

</details><a name="vitals.User.Client.FindADoctor"></a>

##### Client.FindADoctor(userTokenDetail, findADoctorDetail)
<details><summary></summary>

| Param | Type |
| --- | --- |
| userTokenDetail | <code>object</code> | 
| findADoctorDetail | <code>object</code> | 

</details><a name="vitals.User.Client.GetPendingInviteRequestsByUserToken"></a>

##### Client.GetPendingInviteRequestsByUserToken(userTokenDetail, PendingInviteRequestUserTokenQuery)
<details><summary></summary>

| Param | Type |
| --- | --- |
| userTokenDetail | <code>object</code> | 
| PendingInviteRequestUserTokenQuery | <code>object</code> | 

</details><a name="vitals.User.Client.GetPendingInviteRequestsByToken"></a>

##### Client.GetPendingInviteRequestsByToken(userTokenDetail, pendingInviteRequestTokenQuery)
<details><summary></summary>

| Param | Type |
| --- | --- |
| userTokenDetail | <code>object</code> | 
| pendingInviteRequestTokenQuery | <code>object</code> | 

</details><a name="vitals.User.Client.InviteUser"></a>

##### Client.InviteUser(userTokenDetail, inviteUserDetail)
<details><summary></summary>

| Param | Type |
| --- | --- |
| userTokenDetail | <code>object</code> | 
| inviteUserDetail | <code>object</code> | 

</details><a name="vitals.User.Client.LinkUser"></a>

##### Client.LinkUser(userTokenDetail, userLinkDetail)
<details><summary></summary>

| Param | Type |
| --- | --- |
| userTokenDetail | <code>object</code> | 
| userLinkDetail | <code>object</code> | 

</details><a name="vitals.User.Client.UnlinkUser"></a>

##### Client.UnlinkUser(userTokenDetail, userLinkDetail)
<details><summary></summary>

| Param | Type |
| --- | --- |
| userTokenDetail | <code>object</code> | 
| userLinkDetail | <code>object</code> | 

</details><a name="vitals.User.Client.ListUserLink"></a>

##### Client.ListUserLink(UserTokenDetail, UserLinkType)
<details><summary></summary>

| Param | Type |
| --- | --- |
| UserTokenDetail | <code>object</code> | 
| UserLinkType | <code>object</code> | 

</details><a name="vitals.User.Client.ListUserLinkIndividual"></a>

##### Client.ListUserLinkIndividual(UserTokenDetail, UserLinkIndividualDetail)
<details><summary></summary>

| Param | Type |
| --- | --- |
| UserTokenDetail | <code>object</code> | 
| UserLinkIndividualDetail | <code>object</code> | 

</details><a name="vitals.User.Client.ZipLocationLookup"></a>

##### Client.ZipLocationLookup(UserTokenDetail, ZipLocationDetail)
<details><summary></summary>

| Param | Type |
| --- | --- |
| UserTokenDetail | <code>object</code> | 
| ZipLocationDetail | <code>object</code> | 

</details><a name="vitals.User.Client.GetCorrectedAddress"></a>

##### Client.GetCorrectedAddress(UserTokenDetail, getCorrectedAddressDetail)
<details><summary></summary>

| Param | Type |
| --- | --- |
| UserTokenDetail | <code>object</code> | 
| getCorrectedAddressDetail | <code>object</code> | 

</details><a name="vitals.User.Client.GetUserByExternalId"></a>

##### Client.GetUserByExternalId(ExternalIdDetail)
<details><summary></summary>

| Param | Type |
| --- | --- |
| ExternalIdDetail | <code>object</code> | 

</details><a name="vitals.User.Client.ManageSubscriptionsByUserToken"></a>

##### Client.ManageSubscriptionsByUserToken(userTokenDetail, subscriptionDetail)
<details><summary></summary>

| Param | Type |
| --- | --- |
| userTokenDetail | <code>object</code> | 
| subscriptionDetail | <code>object</code> | 

</details><a name="vitals.User.Client.CreateUserExternalIdMapping"></a>

##### Client.CreateUserExternalIdMapping(UserTokenDetail, ExternalIdDetail)
<details><summary></summary>

| Param | Type |
| --- | --- |
| UserTokenDetail | <code>object</code> | 
| ExternalIdDetail | <code>object</code> | 

</details><a name="vitals.User.Client.FindAClinicalTrialLocation"></a>

##### Client.FindAClinicalTrialLocation(UserTokenDetail, FindAClinicalTrialLocationDetail)
<details><summary></summary>

| Param | Type |
| --- | --- |
| UserTokenDetail | <code>object</code> | 
| FindAClinicalTrialLocationDetail | <code>object</code> | 

</details><a name="vitals.User.Client.GenerateExpiringUserToken"></a>

##### Client.GenerateExpiringUserToken(emailAddress)
<details><summary></summary>

| Param | Type |
| --- | --- |
| emailAddress | <code>object</code> | 

</details><a name="vitals.User.Client.GetByExpiringUserToken"></a>

##### Client.GetByExpiringUserToken(expiringUserTokenValue)
<details><summary></summary>

| Param | Type |
| --- | --- |
| expiringUserTokenValue | <code>object</code> | 

</details><a name="vitals.User.Client.SaveUserActivities"></a>

##### Client.SaveUserActivities(userTokenDetail, userActivityDetails)
<details><summary></summary>

| Param | Type |
| --- | --- |
| userTokenDetail | <code>object</code> | 
| userActivityDetails | <code>object</code> | 

</details><a name="vitals.Util"></a>

### vitals.Util
**Properties**

| Name | Type |
| --- | --- |
| Client | [<code>Client</code>](#vitals.Util.Client) | 
| Models | <code>vitals.Util.Models</code> | 

<a name="vitals.Util.Client"></a>

#### Util.Client
<a name="new_vitals.Util.Client_new"></a>

##### new Client(apiDomain, webServiceControlToken, apiToken, clientInfo)
<details><summary></summary>

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
<details><summary></summary>

| Param | Type |
| --- | --- |
| applicationLogDetail | <code>object</code> | 

</details><a name="vitals.Util.Client.GetConfiguration"></a>

##### Client.GetConfiguration(configurationFilters)
<details><summary></summary>

| Param | Type |
| --- | --- |
| configurationFilters | <code>object</code> | 

</details><a name="vitals.Util.Client.SaveJSON"></a>

##### Client.SaveJSON(container, record)
<details><summary></summary>

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

<details><summary></summary>

| Param | Type |
| --- | --- |
| method | <code>\*</code> | 
| result | <code>\*</code> | 

</details>
