# Keyboard Event Key Types

## Description

A simple typescript package that contains the types of keyboard-event-key as string literals forexample: ArrowDown, ArrowUp and so on.
All keys are taken from [developer.mozilla](https://developer.mozilla.org/en-US/docs/Web/API/KeyboardEvent/key/Key_Values#editing_keys.) 
with additional support to custom keys.

The package mainly helps with the IDE-IntelliSense.

## Getting Started
### Installing
```shell
npm install --save keyboard-event-key-type
```

### Usage
```typescript
document.addEventListener('keydown', function ( event ) {
    const actualKey = <KeyboardEventKey>event.key
    const actionKey : KeyboardEventKey = "ArrowDown" // <- intellisense
    if (actualKey === actionKey) {
        // clicked !
    }
})
```

#### IntelliSense
![Alt text](readme_img/IntelliSense.jpg?raw=true "IntelliSense")

## Supported types
All types that are mentioned in https://developer.mozilla.org/en-US/docs/Web/API/KeyboardEvent/key/Key_Values#editing_keys as of 11/19/2021 are supported:
- NumericKeypadKeys 
- UpperAlpha 
- LowerAlpha 
- ModifierKeys 
- WhitespaceKeys 
- NavigationKeys 
- EditingKeys 
- UIKeys 
- DeviceKeys 
- IMECompositionKeys 
- LinuxDeadKeys 
- FunctionKeys 
- PhoneKeys 
- MultimediaKeys 
- TVControlKeys 
- MediaControllerKeys 
- SpeechRecognitionKeys 
- DocumentKeys 
- ApplicationSelectorKeys 
- BrowserControlKeys 
- DeprecatedWhitespaceKey 
- SpecialValueKey 
- CustomValueKey 