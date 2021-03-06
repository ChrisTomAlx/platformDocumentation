## Overview 
Custom directive based on cordova to authenticate users by using the fingerprint or face id (iPhone X) saved on the device. It can be used only on mobiles. If you want to use this add **n-fingerprint** custom directive to any component.

## Usage
This directive is intended to be added to any component. Once added any click event on the component will trigger the following function :-
* A message box asking user to verify his identity using fingerprint or face id.
* Once user verifies his identity using the fingerprint sensor on the mobile a success string is returned.

### How to use   
1. Drag and drop any component and then add the following key-value pairs using the "New property : Attribute" section of the HTML page. Note :- If the value field is missing then leave it empty. If an input needs to be added to the value field, click the slide-toggle button; this makes the value field editable.
    1. Add the directive as key-value pair. Value field is empty here.
        - key : n-fingerprint
        - Leave the value field empty
        - Click the ADD button
    2. Provide the options that the directive will use.
        - key : [fingerprintOptions] 
        - value : `{clientId: 'string', clientSecret: 'string'}`
        - Click the ADD button
    3. Input the action that occurs if the directive successfully completed its functionality.
        - key : (onsuccess)  
        - value : `success($event){console.log($event)}`
        - Click the ADD button
    4. Input the action that occurs if the directive failed to complete its functionality.
        - key : (onerror)  
        - value : `error($event){console.log($event)}`
        - Click the ADD button
2. The `console.log($event)` line inside the values of the (onsuccess) and (onerror) keys can be changed as per the developers requirement. 
>Note :- `console.log($event)` displays the output (which is $event) of the directive for both success and error on a console which can be accessed by google chrome or safari.

## Support
- **Devices:** Android, iOS
- **Browsers:**  None
- **Dependencies version:** 
    - Angular CLI version: 6.0.0 + 
    - Cordova version: 7.1.0 +